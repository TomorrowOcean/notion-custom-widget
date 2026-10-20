# Notion Custom Widget

Single-file widgets meant to be embedded in Notion with an **Embed** block. Each widget lives in its own folder.

| Widget | File | Live page |
|---|---|---|
| Weather | `weather/index.html` | https://tomorrowocean.github.io/notion-custom-widget/weather/ |
| Flip clock | `clock/index.html` | https://tomorrowocean.github.io/notion-custom-widget/clock/ |

Both follow light/dark mode automatically; add `?theme=light` or `?theme=dark` to the URL to lock it.

## Weather

- Weather and city search data come from [Open-Meteo](https://open-meteo.com/) (free, no API key needed); Taiwan-usage Chinese city names come from [Wikidata](https://www.wikidata.org/).
- Shows current conditions and a 7-day forecast for up to 6 cities. Each viewer's city list is saved in their own browser.

## Flip clock

- 24-hour flip clock (hours:minutes) in the viewer's local time, with the date and ISO week number.
- Updates once a minute and pauses while the page is hidden.

## Update

Edit the widget's file, then commit and push to `main`. GitHub Pages redeploys automatically.
To add a widget, put it in a new folder as `index.html`; it is served at `/notion-custom-widget/<folder>/`.
