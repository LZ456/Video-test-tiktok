# DESIGN — 666 Questions (TikTok test series)

## Style Prompt
Cinematic, intimate, late-night. A dark plum-charcoal canvas lit by a single warm rose glow, as if a lamp in a dark room. One emotional line at a time, set in a personal serif with soft hairline rules and quiet ambient drift. Restraint over spectacle — the calm, premium end of TikTok, built to stop the scroll through mood rather than noise.

## Colors
- `--bg`      #140A12  deep plum-charcoal canvas
- `--dip`     #0A0508  near-black used only for the dip-to-black transition
- `--fg`      #F4EBE6  warm off-white (primary text)
- `--muted`   #B79BA6  dusty rose-gray (labels, secondary)
- `--accent`  #FF5D7E  rose — the single accent hue
- `--glow`    #FF9E7A  warm amber-rose for the radial glow only

## Typography
- Display / emotional voice: **Fraunces** (serif, expressive, soft optical)
- Label / interface voice: **Space Grotesk** (sans, distinctive grotesque)
- Extreme weight contrast: 300 vs 800. Headlines 110px+, body 34px+, labels 26px.
- Display tracking -0.03em; light-on-dark body weight 320 with slightly increased line-height.

## Motion
- Primary transition: **color dip to black** (calm/cinematic), 0.5s, `power2`.
- Entrances: `gsap.from` only, 0.5–0.8s, `expo.out` / `power3.out` / `back.out`.
- Ambient: slow glow breathing (scale/opacity), ghost-text drift.
- No exit animations except the final fade to black.

## What NOT to Do
- No cyan/purple neon, no gradient-clipped text, no left accent stripes.
- No pure #000/#FFF. No two similar sans; use one serif + one sans only.
- No busy card grids or UI chrome — this is a mood piece, not a dashboard.
- No emoji. No jump cuts: every scene change is a dip.
