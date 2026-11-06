# Publishing checklist

How to get **OneNote Style** into Obsidian's community theme directory.

## 1. Put the repository on GitHub

Create an empty public repository named `obsidian-onenote-theme` under the `Sundowna` account (no README or license, this repo has them). Then:

```bash
git remote add origin https://github.com/Sundowna/obsidian-onenote-theme.git
git push -u origin main
```

## 2. Make the first release

`version` in `manifest.json` is `1.0.0`. Push a tag with exactly that name, without a `v`:

```bash
git tag 1.0.0
git push origin 1.0.0
```

The **Release** workflow (`.github/workflows/release.yml`) creates the release with `manifest.json` and `theme.css` attached. Obsidian installs the theme from those two files.

## 3. Submit the theme

1. Sign in at [community.obsidian.md](https://community.obsidian.md) and link the GitHub account.
2. Choose **Add your theme** and give the repository `Sundowna/obsidian-onenote-theme`.
3. The review is automatic. If it reports problems, fix them and make a new release (step 4).

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

## 4. Later releases

1. Change the theme in `theme.css`.
2. Raise `version` in `manifest.json` (for example `1.0.1`) and commit.
3. Tag and push: `git tag 1.0.1` then `git push origin main 1.0.1`.

## Rules the directory checks

- The theme name can't change after submission. It must not contain "Obsidian" or "Theme".
- `README.md`, `LICENSE`, `manifest.json` and the screenshot sit in the repository root. The screenshot should be 512 × 288 pixels.
- No remote assets. Fonts and images must be bundled or local. This theme uses only installed fonts.
- Use CSS variables, keep selectors simple and avoid `!important`. This theme has no `!important`.
