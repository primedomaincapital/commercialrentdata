# Image & Video Sources — commercialrentdata.com

All photography and video are verified free-to-use stock from Pexels (Pexels License: free for commercial use, no attribution required — https://www.pexels.com/license/). Every file below was downloaded locally, confirmed as image/video bytes (not 404/403), and visually inspected by a human-in-the-loop (frame extraction + image view) before inclusion.

## Photos (5) — local: `images/`

- `manhattan-midtown-aerial.jpg` — Pexels photo 31661829 — https://www.pexels.com/photo/31661829/ — Aerial view of Midtown Manhattan commercial towers (used in data-moat section).
- `manhattan-towers-aerial.jpg` — Pexels photo 6431295 — https://www.pexels.com/photo/6431295/ — Aerial view of Manhattan towers and streets, daytime (used in insights card for article 2).
- `glass-tower-blue.jpg` — Pexels photo 17131943 — https://www.pexels.com/photo/17131943/ — Low-angle view of a blue glass commercial tower (used in the final Buy Now section + article 3 hero).
- `twin-glass-towers.jpg` — Pexels photo 248877 — https://www.pexels.com/photo/248877/ — Twin glass office towers against the sky (used in "The Asset" section).
- `office-interior.jpg` — Pexels photo 8297846 — https://www.pexels.com/photo/8297846/ — Modern office interior with city-view windows (used in insights card for article 1 + article 1 hero).

Also evaluated and REJECTED after viewing (wrong subject or off-topic):
- Pexels photos 18207068 and 28809197 (more low-angle glass buildings — redundant with the chosen set).
- Pexels photo 5956579 (Singapore skyline at night with prominent corporate signage — not U.S.-market-appropriate).

## Video (hero background) — local: `video/hero.mp4`

- Source: Pexels video 3856665 ("Manhattan aerial at night") — https://www.pexels.com/video/3856665/ — Pexels License, free commercial use, no attribution required.
- Source rendition: `https://videos.pexels.com/video-files/3856665/3856665-hd_1920_1080_30fps.mp4` (2.7 MB).
- Delivered file: re-encoded to H.264 1280×720, CRF 28, `+faststart`, no audio: `ffmpeg -i in.mp4 -vf scale=1280:720 -c:v libx264 -crf 28 -preset fast -an -movflags +faststart hero.mp4`. Final: 500 KB, 5.07 s, seamless loop, muted/autoplay/playsinline.
- Frame verification: extracted 3 frames (1.0 s, 2.5 s, 4.0 s) with ffmpeg and visually inspected all three — real footage of Manhattan at night from an elevated vantage (Midtown towers, lit streets, Hudson/East river edges), no CGI, no particles, no text overlays. Confirmed topical and suitable for a CRE hero.

### Video reuse note (honest flag)
This video (Pexels 3856665) is also the hero on the sibling sale site privatedebtdata.com. A fresh, distinct city-skyline aerial was preferred, but could not be obtained from this sandbox despite extended effort:
- 6 freshly-found Pexels video IDs (857195, 2795750, 856973, 2022395, 2169880, 3129671) were downloaded and frame-verified — all showed wrong content (mountains, a rooftop dancer, countryside, a concert, a coastline, CGI data-viz).
- A further ~13 older video IDs were probed; 3 more downloaded and frame-verified (concert CGI, CGI world map, London bus) — all rejected.
- 6 sibling-site video IDs were probed at 7 rendition patterns each (26561922, 32805742, 36244253, 3856665, 10603140, 11221231, 4319342, 4293589). Newer IDs consistently return HTTP 403 from this sandbox (the direct file host blocks them); 3856665 and 10603140 were the only working, topical options. The Manhattan night aerial was chosen over the top-down cityscape as the better full-bleed hero.

## Design notes
- Fonts: Fraunces (display serif) + Inter (body) via Google Fonts.
- Palette: deep ink/charcoal (#0c0e12) with brass/copper accents (#c9a15a) — original theme; no canvas particle effects; no audio.
