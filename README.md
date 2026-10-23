# Catppuccin for tmarkdown

Soothing pastel themes for [tmarkdown](https://github.com/stephanventer/tmarkdown),
using the [Catppuccin](https://catppuccin.com) palette.

| Theme | Dark | Light |
|---|---|---|
| `catppuccin-mocha` | Mocha | Latte |
| `catppuccin-macchiato` | Macchiato | Latte |
| `catppuccin-frappe` | Frappé | Latte |

## Install

```
git clone <this repo> ~/.config/tmarkdown/themes/catppuccin
```

Then in `~/.config/tmarkdown/config.toml`:

```toml
theme = "catppuccin-mocha"
```

tmarkdown picks dark or light from your terminal background. Use
`appearance = "dark"` or `"light"` (or `--dark` / `--light`) to force one.
tmarkdown doesn't paint the page background, so use a Catppuccin terminal
theme too.

## Colour roles

| tmarkdown role | Catppuccin colour |
|---|---|
| `text` | Text |
| `muted` | Overlay 1 |
| `faint` | Surface 1 |
| `accent_strong` | Mauve |
| `accent` | Blue |
| `accent_soft` | Green |
| `emphasis` | Peach |
| `code_bg` | Mantle |
| `status_bg` | Crust (Latte: Crust) |
| `keycap_bg` | Surface 0 |
| `on_accent` | Crust (Latte: Base) |

Keywords are Mauve, strings Green and links Blue, which matches
Catppuccin's own syntax style. To change the accent, make a theme that
extends one of these:

```toml
# ~/.config/tmarkdown/themes/my-catppuccin.toml
extends = "catppuccin-mocha"

[dark]
accent_strong = "#F5C2E7"   # Pink
```
