# WUWTV Demo Playlist

Premium demo IPTV assets for Apple App Store review, screenshot automation, and ASO templating.

## Playlist URLs

```
https://raw.githubusercontent.com/yucelokan/demo-playlist/main/demo.m3u
https://raw.githubusercontent.com/yucelokan/demo-playlist/main/demo.en-US.m3u
https://raw.githubusercontent.com/yucelokan/demo-playlist/main/demo.tr.m3u
```

## Generate Premium Assets

```sh
python3 scripts/generate_premium_demo_assets.py
```

This command regenerates:

- `demo.en-US.m3u`
- `demo.tr.m3u`
- `demo.en-US.json`
- `demo.tr.json`
- `demo.m3u`
- `demo.json`
- `premium_screenshot_map.json`

## Content

The premium screenshot set is localized for `en-US` and `tr` and follows this structure:

| Type | Categories | Items |
|------|------------|-------|
| 📡 Live TV | 5 | 50 channels |
| 🎬 Movies | 5 | 50 movies |
| 📺 Series | 5 | 50 series / 150 episodes |

Theme: High-Tension, Cinematic, Plot-Twist, Dark Mystery, Action

### Screenshot anchors

- Series dashboard category: `Mind-Bending Thrillers`
- Player / detail anchor movie: `The Seventh Cipher`
- Live category browser: `Premium Sports HD`

## Metadata

Movies and series episodes include: `tvg-description`, `tvg-cast`, `tvg-director`, `tvg-year`, `tvg-rating`, `tvg-genre`, and `tvg-backdrop`.

## Sources

- **Live streams:** public HLS sample streams from Mux and Apple sample feeds
- **VOD streams:** Blender and Google sample assets suitable for test automation
- **Images:** Unsplash Source API

## How to add to WUWTV

1. Open the WUWTV app
2. Tap **Add Playlist**
3. Paste either the `demo.en-US.m3u` or `demo.tr.m3u` raw URL
4. Tap **Load**

The playlist will be parsed automatically — live channels, movies, and series episodes are detected via `tvg-type`.
