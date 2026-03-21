# StarCraft: TMG Companion

A mobile-friendly companion app for StarCraft: The Miniatures Game.

## Features

- **Army Builders** for Zerg, Terran, and Protoss factions
- **Missions & Maps** selector with deployment zones and setup instructions
- **Export** your army lists and battle setups
- **PWA Support** - install on your phone's home screen

## Deployment to GitHub Pages

### Quick Setup

1. Create a new repository on GitHub (e.g., `starcraft-tmg`)

2. Clone and add files:
   ```bash
   git clone https://github.com/YOUR_USERNAME/starcraft-tmg.git
   cd starcraft-tmg
   # Copy all files from this folder into the repo
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

3. Enable GitHub Pages:
   - Go to Settings → Pages
   - Source: Deploy from a branch
   - Branch: main, / (root)
   - Save

4. Your app will be live at: `https://YOUR_USERNAME.github.io/starcraft-tmg/`

### Install on Phone

**iOS (Safari):**
1. Open the site in Safari
2. Tap the Share button (square with arrow)
3. Scroll down and tap "Add to Home Screen"
4. Tap "Add"

**Android (Chrome):**
1. Open the site in Chrome
2. Tap the menu (three dots)
3. Tap "Add to Home screen" or "Install app"
4. Tap "Add"

## Files

- `index.html` - Main hub/splash page
- `zerg.html` - Zerg army builder
- `terran.html` - Terran army builder
- `protoss.html` - Protoss army builder
- `missions.html` - Missions & Maps selector
- `manifest.json` - PWA manifest
- `icon.svg` - App icon

## Updating the Manifest

If your repo name is different from `starcraft-tmg`, update the `start_url` in `manifest.json`:

```json
"start_url": "/YOUR_REPO_NAME/"
```

## Local Testing

Just open `index.html` in a browser. No build step needed!

For PWA features (like install prompts), you'll need to serve over HTTPS or localhost:
```bash
npx serve .
# or
python -m http.server 8000
```

## Credits

Fan-made companion for StarCraft: The Miniatures Game.
StarCraft is a trademark of Blizzard Entertainment.
