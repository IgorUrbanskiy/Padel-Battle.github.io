# Website screenshots

These are real English iOS captures from the prepared Padel Battle store screenshot
set of 18 October 2026. They use demonstration tournament data.

| Website name | Original capture |
| --- | --- |
| `tournament` | `05_round_inplay.png` |
| `standings` | `08_standings_tab.png` |
| `formats` | `02_tournament_formats.png` |
| `setup` | `03_create_players_filled.png` |
| `scores` | `06_score_entry_picker.png` |
| `results` | `09_final_results.png` |

`ios/en/originals/` preserves the 1320 × 2868 PNGs byte for byte. Do not replace
them with smaller exports. Their checksums and original capture names are recorded
in `ios/en/manifest.json`.

The page loads separate 660 × 1434 WebP files, using lossless compression after a
proportional resize. No UI elements, text, scores, or content have been altered.
The six WebP files together are about 241 KB. Full-resolution images open when
a visitor selects a screenshot in the formats or walkthrough sections.

To regenerate one web export with libwebp installed, run from the repository root:

```sh
cwebp -lossless -z 9 -resize 660 0 -metadata none \
  assets/screenshots/ios/en/originals/tournament.png \
  -o assets/screenshots/ios/en/tournament.webp
```

Phone framing and placement are CSS. Future platform or language versions should
have their own folders and labels, using the corresponding real app captures.
