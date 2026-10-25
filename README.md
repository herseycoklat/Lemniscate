# Lemniscate

Portfolio site for Lemniscate — games, stories and music.

> The creative mind is infinite in its potential.
> Your emotion is what drives your impact.
> Deep inside you always had it in you.

## What's here

| Path | Contents |
|---|---|
| `index.html` | The whole site — one self-contained page (styles, scripts and logo are inline) |
| `demos/` | Short gameplay clips (`.mp4`) and poster frames (`.jpg`) shown in the Works carousel and hover previews |
| `audio/` | Music tracks played by the Sound deck |

No build step. Any static host serves it as-is.

## Run locally

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

Open it through a local server rather than double-clicking the file — the music visualiser needs the audio to come from the same origin.

## Deploy (Netlify)

1. New site → Import from GitHub → pick this repo.
2. Build command: *(leave empty)* · Publish directory: `.`
3. Deploy. `netlify.toml` already sets long cache headers for the media.

## Updating content

- **Games** — rows live in the `#works` section; carousel cards in `#show`. Each game has its own theme class (`g-nak`, `g-laz`, `g-cov`, `g-ef`).
- **Writing** — manuscript cards are in `.folio`; essays open from the `<article class="essay">` blocks near the bottom.
- **Music** — tracks are `<li class="trk">` entries; waveform shapes are in the `PEAKS` object in the script.

## Credits

- Music: *The Island* and *Guardian of Stone* for The Divine Vault by UPHC Boardgames (@boardgames.uphc). *Intoxicating Gamelan* released as NAKULONG.
- *The Covenant* is a collaboration with Clozy (@curesorrow).
