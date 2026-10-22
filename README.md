# Color Pocket: GitHub Pages five-cartridge player

Portrait shows a Game Boy Color-inspired console. Landscape hides the shell and shows translucent controls over the game. Select a cartridge and press Play to load a ROM directly from the GitHub Pages site.

## Publish
1. Create a GitHub repository and upload `index.html` and the `games/` directory.
2. In Settings → Pages, deploy from the `main` branch at `/ (root)`.
3. **Only if you have permission to distribute the game files**, add the corresponding ROMs to `games/` with these exact filenames:
   - `red.gb`, `blue.gb`, `yellow.gb`
   - `silver.gbc`, `gold.gbc`
4. Visit your GitHub Pages URL, select a cartridge, and tap Play.

**Copyright:** No commercial Pokémon ROMs are supplied. Owning a cartridge does not generally grant permission to redistribute its ROM publicly. If you cannot host those ROMs legally, use a local-ROM-loader design instead.

## Notes
- EmulatorJS assets load from a CDN; network access is required.
- Games without a matching file display an error rather than loading.
- The custom touch controls use synthetic keyboard events, which may not work in every EmulatorJS version, particularly on iOS. Test before relying on them.
- Save through the emulator menu before switching cartridges. Browser save behavior depends on EmulatorJS and browser storage.
- The emulator has not been device-tested here.
