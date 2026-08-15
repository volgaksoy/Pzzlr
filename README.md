# Puzzlr

A browser-based physical jigsaw puzzle game. Create a puzzle from an online or local image, crop it, choose a difficulty, optionally rotate pieces, and save sessions locally in the browser.

## Play locally

Puzzlr is a static site, so there is nothing to compile and no package installation is required. You only need Python 3 to run the included local server.

```bash
git clone https://github.com/volgaksoy/Pzzlr.git
cd Pzzlr
```

On Windows, double-click `start-local.cmd` or run:

```powershell
.\start-local.cmd
```

On macOS or Linux, run:

```bash
./start-local.sh
```

The launcher serves the repository at `http://127.0.0.1:8000/` and opens it in your default browser. Press `Ctrl+C` in the terminal to stop it.

You can choose another port or prevent the browser from opening automatically:

```bash
python3 serve.py --port 8080 --no-browser
```

Do not open `index.html` directly as a `file://` URL; browser security rules can interfere with image loading and other app features.

## Hosting

The site is designed to run directly from GitHub Pages with no build step.
