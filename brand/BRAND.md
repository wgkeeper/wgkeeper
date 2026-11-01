# wgkeeper brand

The logo is the wordmark itself: **wg** in bold brand red, **keeper** in regular ink. Products add their name in regular muted grey: **wgkeeper node**, **wgkeeper console**. The square **wg** icon is for places that need a small square image: favicons, avatars, app icons.

The files in this folder are the single source for every repository and the docs site. READMEs link to them by URL, so **never rename or move a file here**; add a new one instead.

## Files

| File | Use |
| --- | --- |
| `wgkeeper-light.svg`, `wgkeeper-dark.svg` | Wordmark, for the umbrella repo and the docs site |
| `wgkeeper-node-light.svg`, `wgkeeper-node-dark.svg` | Node README header |
| `wgkeeper-console-light.svg`, `wgkeeper-console-dark.svg` | Console README header and app header |
| `icon-light.svg`, `icon-dark.svg` | Square icon: dark tile for light backgrounds, light tile for dark ones |
| `favicon.svg` | Favicon; switches tile colour with the browser theme by itself |
| `avatar.png` | 512 × 512 avatar for the GitHub organisation and Docker Hub |
| `social.png`, `social-node.png`, `social-console.png` | 1280 × 640 GitHub social previews (Settings → Social preview) |

`-light` files are for light backgrounds, `-dark` for dark ones. In a README, add both and let GitHub show the one that matches the viewer's GitHub theme:

```html
<p align="center">
  <img alt="wgkeeper node" src="https://raw.githubusercontent.com/wgkeeper/wgkeeper/main/brand/wgkeeper-node-light.svg#gh-light-mode-only" height="64"><img alt="wgkeeper node" src="https://raw.githubusercontent.com/wgkeeper/wgkeeper/main/brand/wgkeeper-node-dark.svg#gh-dark-mode-only" height="64">
</p>
```

Keep both `<img>` tags on one line with no space between them, so the visible one stays centred. Don't use `<picture>` with `prefers-color-scheme`: it follows the operating system's theme, not GitHub's, and shows the wrong file when the two differ.

## Colour

Taken from the console's theme tokens (`--brand`, `--foreground`), so the app and the logo match.

| Role | Light background | Dark background |
| --- | --- | --- |
| Brand red (`wg`) | `#E01729` · `oklch(0.577 0.225 25.3)` | `#F54846` · `oklch(0.65 0.21 25.6)` |
| Ink (`keeper`) | `#0A0A0A` | `#FAFAFA` |
| Muted (product name) | `#6B6B6B` | `#A1A1A1` |
| Icon tile | `#171717` | `#FAFAFA` |

Red is an accent: it appears on `wg` and nowhere else in the logo. Keep it off large areas, where it reads as an error.

## Type

[Geist](https://vercel.com/font) (SIL Open Font License), the console's interface face. In the SVGs the letters are converted to outlines, so they render the same without the font installed.

- `wg`: Geist Bold
- `keeper` and the product name: Geist Regular
- Letter spacing −0.035 em; the product name is separated by a 0.24 em gap.

## Writing the name

Always lowercase, in the logo and in running text alike: **wgkeeper**, **wgkeeper node**, **wgkeeper console**. Not WGKeeper, WgKeeper or WG Keeper. Keep it lowercase at the start of a sentence too ("wgkeeper runs…"), and in code, packages and images: `wgkeeper`, `wgkeeper-node`, `ghcr.io/wgkeeper/node`.

## Don't

- Recolour `wg` or `keeper`, or swap their weights.
- Set the wordmark in another typeface or redraw it as live text.
- Put the light version on a dark background or the reverse.
- Add effects: outlines, shadows, gradients.
- Stretch, rotate or crowd it: leave at least the height of the `w` clear on every side.

WireGuard® is a registered trademark of Jason A. Donenfeld.
