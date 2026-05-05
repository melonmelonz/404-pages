# 404-pages

A small collection of distinctive, drop-in `404.html` pages.

Each file is single-file, zero-build HTML — pixel art is inline SVG, animations are CSS, fonts are loaded from Google Fonts. Save one as `404.html` in your site root and your host will serve it for missing routes.

## The pages

| File | Vibe |
|---|---|
| [`missingno.html`](./missingno.html) | Glitched Gen-1 Pokémon battle screen. Cycling sprite frames, broken HP bar, typewriter text, ▶ RUN cursor blink. |
| [`snorlax.html`](./snorlax.html) | Top-down route. Sleeping creature blocks the path. Breathing animation, drifting Z particles, swaying grass, "!" bubble. |
| [`rocket.html`](./rocket.html) | Starry night over a city skyline. Two silhouettes blasting off diagonally toward a sparkle ding. Parallax stars. |
| [`lavender.html`](./lavender.html) | Quiet haunted tower. Translucent ghost bobbing and fading, blinking windows, drifting music notes, echoing 404. |
| [`terminal.html`](./terminal.html) | Green-phosphor terminal. `cd /the-page` returns "No such file or directory," ASCII error box, blinking cursor on `cd /home`. |
| [`tombstone.html`](./tombstone.html) | Aged paper. ASCII tombstone with epitaph "born: ?, found: never." Special Elite typewriter font. |
| [`shrug.html`](./shrug.html) | Pure minimalism. Big `¯\_(ツ)_/¯`, "404", and one line: "we looked. it's not here. could be anywhere." |
| [`goolz-society.html`](./goolz-society.html) | Quiet Victorian field-society 404. Paper background, ASCII art, no JS. The original. |
| [`next-chapter-bsod.html`](./next-chapter-bsod.html) | Authentic Win9x BSOD. Backspace=back, Enter=home, blinking cursor. |

A live gallery is in [`index.html`](./index.html).

## How to use

### Cloudflare Pages, Netlify, GitHub Pages
Drop the file as `404.html` in the root of your published directory.

### Nginx
```nginx
error_page 404 /404.html;
```

### Apache
```apache
ErrorDocument 404 /404.html
```

## Switching between pages on one site

If you want different sections of your site to serve different 404s — e.g. the marketing pages get the Society version and the desktop app gets the BSOD — combine them and switch on `location.pathname`. The [original goolz 404](https://github.com/melonmelonz/goolz/blob/main/404.html) does exactly that.

## Notes on the art

All pixel sprites are original SVGs drawn for this project, in tribute to the Gen-1 Game Boy palette and Lavender Town aesthetic. Names like "MissingNo," "Snorlax," and "Lavender Town" are referenced as cultural touchstones — no original sprite assets are copied.

GB green palette: `#0f380f` `#306230` `#8bac0f` `#9bbc0f`
Lavender palette: `#0e0518` `#1f0e34` `#3a1f5c` `#6b3da6` `#b487d4` `#f0d4f8`

## License

MIT. Use them, fork them, tweak them.

— [penn @ goolz.org](https://goolz.org)
