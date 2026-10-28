# SLCM AutoFeedback

A tiny Chrome / Edge extension for **Manipal University Jaipur (MUJ) SLCM** that adds two buttons to the faculty feedback form:

- **✔ All YES** – selects YES for every question
- **✖ All NO** – selects NO for every question

You can still change individual answers before submitting. The extension never submits anything on its own.

## Install

1. Download this repo: **Code → Download ZIP**, then extract it.
2. Open `chrome://extensions` (Chrome) or `edge://extensions` (Edge).
3. Turn on **Developer mode**.
4. Click **Load unpacked** and select the **`extension`** folder (the one containing `manifest.json`).

> "Manifest file is missing or unreadable" means you selected the wrong folder — pick the one that directly contains `manifest.json`.

## Use

1. Log in to [SLCM](https://mujslcm.jaipur.manipal.edu) and open **Feedback**.
2. Click a **Pending** course to open its form.
3. Click **All YES** or **All NO** (bottom-right), review, then **Submit**.
4. Repeat for each faculty.

The buttons only appear on pages that have YES/NO options, so you won't see them on the feedback list.

## Updating

Replace the files, click the reload icon on the extension in `chrome://extensions`, then refresh SLCM.

## Privacy

- Runs only on `mujslcm.jaipur.manipal.edu`.
- No network requests, no data collection, no special permissions. All the code is in [`extension/content.js`](extension/content.js).

## Troubleshooting

If the button shows **"Selected 0"**, the SLCM page layout has probably changed. Open an issue with a screenshot of a YES button's HTML (right-click → Inspect).

## Disclaimer

Unofficial student project, not affiliated with or endorsed by Manipal University Jaipur. Feedback matters to faculty, so use it responsibly and review your answers before submitting.

## License

[MIT](LICENSE)
