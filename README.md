# WUWTV Demo Playlist

A copyright-free demo IPTV playlist for Apple App Store review and testing purposes.

## Playlist URL

```
https://raw.githubusercontent.com/yucelokan/demo-playlist/main/demo.m3u
```

## Content (v5)

All content is copyright-free / CC0 / public test streams — safe for App Store review:

| Type | Groups | Entries |
|------|--------|---------|
| 📡 Live TV | Nature & Wildlife, Space & Science, World Documentary, Arts & Culture, Kids & Education, Travel & Adventure, History & Heritage, Technology & Innovation, Sports & Fitness, Music & Lifestyle | **100 channels** |
| 🎬 Movies | Nature Documentary, Space & Sci-Fi, Adventure, Animation, Drama, History, Mystery & Thriller, Family, Crime, Romance | **100 films** |
| 📺 Series | 10 genre categories × 10 series × 3 episodes | **300 episodes** (100 unique series) |

**Total: 500 entries**

### Series genre categories (10)

| Genre | Series count |
|-------|-------------|
| Documentary | 10 |
| Crime | 10 |
| Sci-Fi | 10 |
| Mystery | 10 |
| Drama | 10 |
| Adventure | 10 |
| Animation | 10 |
| History | 10 |
| Romance | 10 |
| Thriller | 10 |

### Rich metadata per entry

Movies and series episodes include: `tvg-description`, `tvg-cast`, `tvg-director`, `tvg-year`, `tvg-rating`, `tvg-genre`, `tvg-backdrop`

## Sources

- **Live streams:** [Mux](https://test-streams.mux.dev/) public HLS test stream & [Apple Developer](https://developer.apple.com/streaming/examples/) HLS sample streams (Big Buck Bunny, CC-BY)
- **Images:** [Picsum Photos](https://picsum.photos/) via CDN (CC0, no attribution required)
  - Live logos: 400×225 (landscape) — `picsum.photos/id/{n}/400/225`
  - Movie / Series covers: 300×450 (portrait) — `picsum.photos/id/{n}/300/450`
  - Backdrops: 800×450 — `picsum.photos/id/{n}/800/450`

## How to add to WUWTV

1. Open the WUWTV app
2. Tap **Add Playlist**
3. Paste the raw URL above
4. Tap **Load**

The playlist will be parsed automatically — live channels, movies, and series episodes are detected via `tvg-type`.
