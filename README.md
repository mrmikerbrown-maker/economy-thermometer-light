# Economy thermometer LIGHT

A light, Macro Perspective-styled version of the "Is the economy hot or cold?" spiral chart:
inflation against growth (or unemployment) over the business cycle, for the G10 economies.

- `index.html` is the page. It only draws what is in `data.json`.
- `scripts/update.py` fetches the data (BIS, FRED, Eurostat) and writes `data.json`.
  Run `python scripts/update.py --demo` to test it on made-up data with no internet.
- `.github/workflows/update.yml` runs the update every day at about 07:17 UK time and refreshes the page.
- Link straight to a country with `#uk`, `#us`, `#ea`, `#jp` and so on at the end of the address.

This is a separate copy of economy-thermometer, trimmed to the spiral view only. Fixes made in
one repo do not reach the other automatically.

## Turning the page on (one time)

1. Settings → Pages → "Deploy from a branch" → branch `main`, folder `/ (root)` → Save.
2. The page appears at https://mrmikerbrown-maker.github.io/economy-thermometer-light/ within a minute or two.
