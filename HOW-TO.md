# Home-screen icon for BCI Staff app

Google does not let an Apps Script link carry its own home-screen icon. That is why the iPhone shows a plain "B".
This small launcher page fixes it: it carries the BCI icon and name, and opens your app inside it.

## Step 1 – Put your app link in
Open `index.html` in Notepad. Find `PASTE_YOUR_EXEC_LINK_HERE` and paste your app link (the one ending in `/exec`) between the quotes. Save.

## Step 2 – Put it online free (GitHub Pages, 10 minutes, one time)
1. Go to github.com and create a free account.
2. Click **+ → New repository**. Name: `bci-staff`. Select **Public**. Click **Create repository**.
3. Click **uploading an existing file**. Drag in all files from this folder: `index.html`, `manifest.webmanifest` and the 4 `.png` files. Click **Commit changes**.
4. Go to **Settings → Pages**. Under "Branch" choose **main** and **/(root)**, click **Save**.
5. After 1–2 minutes your link appears there, like `https://yourname.github.io/bci-staff/`.

## Step 3 – Share the new link with teachers
- **iPhone:** open the new link in Safari → Share → **Add to Home Screen**.
- **Android:** open in Chrome → ⋮ menu → **Add to Home screen** / **Install app**.
Delete the old "B" shortcut first.

## Use your own logo instead
Replace the 4 PNG files with your logo, keeping the same file names and sizes:
`apple-touch-icon.png` 180×180, `icon-192.png` 192×192, `icon-512.png` 512×512, `icon-maskable-512.png` 512×512 (logo smaller, with space around it).
Use a square image with a solid background (no transparency) – iPhone shows transparent areas as black.

## Notes
- The grey line "This application was created by a Google Apps Script user" is added by Google on free Gmail accounts and cannot be removed.
- If the app ever does not load inside the launcher, a "Open directly" button appears after a few seconds.
- When you deploy a new version of the app, the /exec link stays the same, so you never need to change this page again.
