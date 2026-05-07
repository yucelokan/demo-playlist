# WUWTV Demo Playlist

Premium demo IPTV assets for Apple App Store review, screenshot automation, and ASO templating.

## Playlist URLs

```
https://raw.githubusercontent.com/yucelokan/demo-playlist/feature/aso-master-assets/demo.m3u
https://raw.githubusercontent.com/yucelokan/demo-playlist/feature/aso-master-assets/demo.en-US.m3u
https://raw.githubusercontent.com/yucelokan/demo-playlist/feature/aso-master-assets/demo.tr.m3u
```

These URLs point at the current TMDB-based ASO dataset. Do not use the `main` branch raw URLs for screenshot testing because `main` still serves older playlist content.

## Generate Premium Assets

```sh
TMDB_API_KEY=YOUR_KEY python3 scripts/generate_premium_demo_assets.py
```

Or pass credentials explicitly:

```sh
python3 scripts/generate_premium_demo_assets.py --api-key YOUR_KEY
```

This command regenerates:

- `demo.en-US.m3u`
- `demo.tr.m3u`
- `demo.en-US.json`
- `demo.tr.json`
- `demo.m3u`
- `demo.json`
- `premium_screenshot_map.json`
- `screenshot_config.aso-master.json`

## Content

The premium screenshot set is localized for `en-US` and `tr` and follows this structure:

| Type | Categories | Items |
|------|------------|-------|
| 📡 Live TV | 5 | 50 channels |
| 🎬 Movies | 5 | 50 movies |
| 📺 Series | 5 | 50 series / 150 episodes |

Playlist version: `aso-master-v2`

Theme: high-tension, plot-twist, dark mystery, sci-fi, action

### Screenshot anchors

- Series dashboard category: `Mind-Bending Thrillers`
- Player / detail anchor movie: `Tears of Steel`
- Live category browser: `Premium Sports` / `Premium Spor`

## Metadata

Movies and series episodes include: `tvg-description`, `tvg-cast`, `tvg-director`, `tvg-year`, `tvg-rating`, `tvg-genre`, and `tvg-backdrop`.

## Sources

- **Playback URL:** every live, movie, and episode entry resolves to the same public Sintel stream for deterministic screenshot playback
- **Movie/series metadata and artwork:** TMDB
- **Live channel logos:** UI Avatars

## How to add to WUWTV

1. Open the WUWTV app
2. Tap **Add Playlist**
3. Paste either the `demo.en-US.m3u` or `demo.tr.m3u` raw URL
4. Tap **Load**

If you imported an older demo playlist before, remove it first or bump the playlist version in the app flow; otherwise WUWTV may continue showing cached legacy content.

The playlist will be parsed automatically. Live channels, movies, and series episodes are detected via `tvg-type`.
