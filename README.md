# WUWTV Demo Playlist

A copyright-free demo IPTV playlist for Apple App Store review and testing purposes.

## Playlist URL

```
https://raw.githubusercontent.com/yucelokan/demo-playlist/main/demo.m3u
```

## Content (v4)

All content is copyright-free / CC0 / public test streams — safe for App Store review:

| Type | Groups | Entries |
|------|--------|---------|
| 📡 Live TV | Nature & Wildlife, Space & Science, World Documentary, Arts & Culture, Kids & Education, Travel & Adventure, History & Heritage, Technology & Innovation, Sports & Fitness, Music & Lifestyle | **100 channels** |
| 🎬 Movies | Nature Documentary, Space & Sci-Fi, Adventure, Animation, Drama, History, Mystery & Thriller, Family, Crime, Romance | **100 films** |
| 📺 Series | Wild Planet, Cosmos Journey, Ancient Empires, Ocean Depths, True North, Case Files, Night Watch, Digital Minds, Star Wanderers, Mystery Cove | **60 episodes** (10 series × 6 eps) |

**Total: 260 entries**

### Series genre grouping

| Genre (first token) | Series |
|---------------------|--------|
| Documentary | Wild Planet, Cosmos Journey, Ancient Empires, Ocean Depths |
| Crime | True North, Case Files, Night Watch |
| Sci-Fi | Digital Minds, Star Wanderers |
| Mystery | Mystery Cove |

## Sources

- **Live streams:** [Mux](https://test-streams.mux.dev/) public HLS test stream & [Apple Developer](https://developer.apple.com/streaming/examples/) HLS sample streams (Big Buck Bunny, CC-BY)
- **Images:** [Lorem Picsum](https://picsum.photos/) (CC0, no attribution required)
  - Live logos: 400×225 (landscape)
  - Movie / Series covers: 300×450 (portrait)
  - Backdrops: 800×450

## How to add to WUWTV

1. Open the WUWTV app
2. Tap **Add Playlist**
3. Paste the raw URL above
4. Tap **Load**

The playlist will be parsed automatically — live channels, movies, and series episodes are detected via `tvg-type`.
