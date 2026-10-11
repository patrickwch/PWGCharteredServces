# Melbourne Airport Arrivals Guide

A one-page website that shows arriving passengers how to get from the arrivals hall to the Pick Up zone at Melbourne Airport, following the changes that took effect on 6 October 2026. The page is in English and Simplified Chinese, with a switch at the top.

## What is in this folder

| File | What it is |
| --- | --- |
| `index.html` | The whole page: text in both languages, styling and the language switch. |
| `img/` | The 14 step pictures: seven with English labels (`-en.jpg`) and seven with Chinese labels (`-zh.jpg`). |
| `README.md` | This file. |

Keep `index.html` and the `img` folder together. The page looks for the pictures at `img/…`, so they will not show if the folder is moved or renamed.

## Publishing on GitHub Pages

1. Create a new repository on GitHub (public, unless your plan allows Pages on private repositories).
2. Upload `index.html`, the `img` folder and `README.md` to the top level of the repository. Dragging the folder contents into "Add file → Upload files" keeps the `img` folder intact.
3. Open **Settings → Pages**. Under "Build and deployment", choose **Deploy from a branch**, select the `main` branch and the `/ (root)` folder, then save.
4. After a minute or two the site is live at `https://<your-username>.github.io/<repository-name>/`.

## Language links

- The page opens in Chinese for visitors whose browser is set to Chinese, and in English for everyone else. It remembers each visitor's choice.
- To send a client straight to one language, add `#zh` or `#en` to the end of the link, for example `https://<your-username>.github.io/<repository-name>/#zh`.

## Editing the page

- **Text:** open `index.html` in a text editor. Every piece of text appears twice, once in an element with `class="en"` and once with `class="zh"`. Change both so the two languages stay in step.
- **Terminal picker answers:** these are in the `<script>` block at the bottom of `index.html`, in the `data` object, again with an `en` and a `zh` version of each line.
- **Pictures:** replace a file in `img/` with a new one of the same name. The pictures are 1182 × 665 pixels; keep the same proportions so the layout does not shift.

## Things to know

- **Fonts:** the English fonts load from Google Fonts. Without an internet connection the page falls back to standard system fonts. Chinese text uses the fonts already on the visitor's device.
- **Pictures:** these are computer-generated stills from Melbourne Airport's official walking route video (https://www.youtube.com/watch?v=gWbqixtnvJE), with arrows and labels added. The images are © Melbourne Airport. Check you have their permission before publishing them publicly.
- **Chinese translation:** this has not been reviewed by a native speaker. Sign names such as "T123 Transport Hub" and "T123 Pick-up" are left in English on purpose so they match the real signs.
- **Keeping it current:** details were taken from Melbourne Airport's website on 11 October 2026. Arrangements may change as the Terminal 2 expansion proceeds, so recheck https://www.melbourneairport.com.au/pick-up-and-drop-off-hub from time to time and update the date in the page footer.
- **Estimates:** the "5 to 10 minutes" walking time is our own estimate. The airport states only the distance, about 285 metres.
