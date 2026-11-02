# PocketPal

Know what you can spend today. PocketPal turns your monthly budget into one number a day, rolls over at midnight, and moves whatever you don't spend into a saving buffer.

No login. Data is saved on your device, in your browser. Works offline once opened.

## Use it on your phone

1. In this repository, go to **Settings → Pages**, choose **Deploy from a branch**, pick **main** and **/(root)**, and save.
2. After a minute, open `https://navisharai-design.github.io/PocketPal/` on your phone.
3. Install it:
   - **Android (Chrome):** ⋮ menu → **Install app** / **Add to Home screen**
   - **iPhone (Safari):** Share → **Add to Home Screen**

GitHub Pages on a free account needs the repository to be public.

## Run it on your computer

Offline support and installing need the app to be served from a web address, not opened as a file.

```
cd PocketPal
python3 -m http.server 8000
```

Then open http://localhost:8000. Opening `index.html` directly also works for trying it out, but it won't install or work offline.

## Files

| File | What it does |
| --- | --- |
| `index.html` | The whole app: screens, budget engine, storage |
| `manifest.webmanifest` | App name, colours and icons used when installing |
| `sw.js` | Caches the app so it opens without internet |
| `icons/` | Home screen and browser icons |

## Your data

- Saved in the browser's local storage on each device. Nobody else can see it.
- Clearing browser data for the site deletes it, so use **Settings → Export and backup** to download a backup file now and then. You can restore it on a new phone from the same screen.
- **Download CSV** gives you every payment for Excel or Google Sheets.
