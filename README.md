# Guitar Tuner

A single-page guitar tuner web app for GitHub Pages. The app lives entirely in `index.html` with inline CSS and JavaScript, no build tools, no dependencies, and no CDN imports.

## Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

Open `index.html` in a browser for local testing. Microphone access works best from `https://` or `localhost`; GitHub Pages serves the deployed site over HTTPS.

## Enable GitHub Pages

1. Push this repository to GitHub.
2. Open the repository on GitHub.
3. Go to **Settings**.
4. Select **Pages** in the sidebar.
5. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
6. Set the branch to **main** and the folder to **/root**.
7. Click **Save**.

GitHub will publish the app at the Pages URL shown on that settings page.

## Use a Scarlett Solo as the Default Input

### Windows

1. Connect the Scarlett Solo and install Focusrite Control or the current Focusrite driver if Windows has not already configured it.
2. Right-click the speaker icon in the taskbar and open **Sound settings**.
3. Under **Input**, choose **Scarlett Solo USB**.
4. Click the selected input device and confirm the input level moves when you play.
5. In Chrome or Firefox, open the tuner and allow microphone access when prompted.

If the browser picked a different microphone earlier, open the site permissions from the icon in the address bar, reset the microphone permission, then start the tuner again.

### macOS

1. Connect the Scarlett Solo.
2. Open **System Settings**.
3. Go to **Sound**.
4. Open the **Input** tab.
5. Select **Scarlett Solo USB**.
6. Play your guitar and confirm the input level meter moves.
7. In Chrome or Firefox, open the tuner and allow microphone access when prompted.

If macOS blocks browser microphone access, open **System Settings -> Privacy & Security -> Microphone** and enable access for Chrome or Firefox.

## Tuning Notes

The A4 reference slider ranges from 430 Hz to 450 Hz in 0.5 Hz steps. The six standard guitar string targets, E2, A2, D3, G3, B3, and E4, recalculate automatically whenever A4 changes.
