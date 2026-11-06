# Publishing checklist

How to release **OneNote Style** and keep it listed in Obsidian's community theme directory.

The repository is https://github.com/Sundowna/obsidian-onenote-theme.

## Releases

Obsidian installs the theme from the GitHub release whose tag equals `version` in `manifest.json` (no `v` in front). That release must have `manifest.json` and `theme.css` attached.

To make a new release:

1. Change the theme in `theme.css`.
2. Raise `version` in `manifest.json` (for example `1.0.1`) and commit.
3. Push and release with the GitHub CLI:

```bash
git push
```

```bash
gh release create 1.0.1 manifest.json theme.css --title 1.0.1 --generate-notes
```

## Submit the theme (once)

1. Add `screenshot.png` (512 × 288) to the repository root and push it.
2. Sign in at [community.obsidian.md](https://community.obsidian.md) and link the GitHub account.
3. Choose **Add your theme** and give the repository `Sundowna/obsidian-onenote-theme`.
4. The review is automatic. If it reports problems, fix them and make a new release.

For the older pull-request route, this is the entry for `community-css-themes.json` in `obsidianmd/obsidian-releases`:

```json
{
  "name": "OneNote Style",
  "author": "Sundowna",
  "repo": "Sundowna/obsidian-onenote-theme",
  "screenshot": "screenshot.png",
  "modes": ["dark", "light"]
}
```

## Rules the directory checks

- The theme name can't change after submission. It must not contain "Obsidian" or "Theme".
- `README.md`, `LICENSE`, `manifest.json` and the screenshot sit in the repository root. The screenshot should be 512 × 288 pixels.
- No remote assets. Fonts and images must be bundled or local. This theme uses only installed fonts.
- Use CSS variables, keep selectors simple and avoid `!important`. This theme has no `!important`.
