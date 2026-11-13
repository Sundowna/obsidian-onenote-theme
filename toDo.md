# To do

## Before submitting to the community theme store

- [x] **Screenshot.** `screenshot.png` (512 × 288) is in the repo root, taken from a demo vault with sample notes (2026-11-13). It shows the theme with the OneNote Style plugin's ribbon. The README has five pictures from `docs/`: three with the ribbon, two with the theme alone.
- [ ] **Check the theme in Obsidian.** Look at it in light and dark mode:
  - The title row, left icon strip and the Minimise / Maximise / Close buttons are one colour.
  - The open tab reads as part of the page, with its close button visible.
  - The sidebar tab icons and the active file in the file list.
  - Headings, highlights, tables, quotes and to-do boxes.
- [ ] **Check the Style Settings options:** slate and neutral title row, grey side panes, plain headings, and Obsidian's fonts.
- [x] **Check alongside the OneNote Style plugin.** With plugin 2.0.0 the ribbon's tab row, the title row and the window buttons are one colour in light mode (checked 2026-11-13, see `docs/1-ribbon-light.png`). The slate and neutral options were not rechecked.
- [ ] **Submit.** Sign in at [community.obsidian.md](https://community.obsidian.md), choose **Add your theme** and enter `Sundowna/obsidian-onenote-theme`.

## Later

- [ ] **Automatic releases.** Bring back the GitHub Actions workflow that releases on a tag push. Pushing it needs a GitHub sign-in with the `workflow` scope: `gh auth refresh -s workflow`.
- [x] **Dark mode screenshot.** `docs/2-ribbon-dark.png` and `docs/5-theme-dark.png` are in the README.
- [ ] **More Style Settings options** if people ask: page colour, ruled lines, accent colour presets.
- [ ] **Smaller screens.** Check the theme on a narrow window and on Obsidian mobile.

## Done

- [x] Theme with light and dark modes, no remote assets and no `!important`.
- [x] `manifest.json`, `README.md`, MIT `LICENSE` and a publishing checklist.
- [x] Public repository on GitHub.
- [x] Release 1.0.0 with `theme.css` and `manifest.json`.
