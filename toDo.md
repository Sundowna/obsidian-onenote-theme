# To do

## Before submitting to the community theme store

- [ ] **Screenshot.** Add `screenshot.png` (512 × 288) to the repo root. Take it from a demo vault with harmless sample notes, not a real vault. The README already links it.
- [ ] **Check the theme in Obsidian.** Look at it in light and dark mode:
  - The title row, left icon strip and the Minimise / Maximise / Close buttons are one colour.
  - The open tab reads as part of the page, with its close button visible.
  - The sidebar tab icons and the active file in the file list.
  - Headings, highlights, tables, quotes and to-do boxes.
- [ ] **Check the Style Settings options:** slate and neutral title row, grey side panes, plain headings, and Obsidian's fonts.
- [ ] **Check alongside the OneNote Style plugin.** The plugin's purple bar and the theme's title row should sit together cleanly, including with the slate option.
- [ ] **Submit.** Sign in at [community.obsidian.md](https://community.obsidian.md), choose **Add your theme** and enter `Sundowna/obsidian-onenote-theme`.

## Later

- [ ] **Automatic releases.** Bring back the GitHub Actions workflow that releases on a tag push. Pushing it needs a GitHub sign-in with the `workflow` scope: `gh auth refresh -s workflow`.
- [ ] **Dark mode screenshot.** A second picture for the README.
- [ ] **More Style Settings options** if people ask: page colour, ruled lines, accent colour presets.
- [ ] **Smaller screens.** Check the theme on a narrow window and on Obsidian mobile.

## Done

- [x] Theme with light and dark modes, no remote assets and no `!important`.
- [x] `manifest.json`, `README.md`, MIT `LICENSE` and a publishing checklist.
- [x] Public repository on GitHub.
- [x] Release 1.0.0 with `theme.css` and `manifest.json`.
