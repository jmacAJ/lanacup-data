# Lanacup data

Public static data snapshots for the Lanacup World Cup predictor.

Generated from private predictor repo commit `c55c6a8`.

## Files

- `data/latest.json` — canonical latest JSON snapshot for applets/backends.
- `data/worldcup_predictor_data.json` — same current snapshot, kept at the stable predictor export name.
- `js/lanacup_data.js` — JavaScript bundle that sets `window.LANACUP_DATA` for standalone/static applets.
- `manifest.json` — metadata/checksum for the current snapshot.

## Raw URLs

```text
https://raw.githubusercontent.com/jmacAJ/lanacup-data/main/data/latest.json
https://raw.githubusercontent.com/jmacAJ/lanacup-data/main/js/lanacup_data.js
https://raw.githubusercontent.com/jmacAJ/lanacup-data/main/manifest.json
```

## Usage in a static applet

Fetch JSON:

```js
const url = "https://raw.githubusercontent.com/jmacAJ/lanacup-data/main/data/latest.json";
const data = await fetch(url, { cache: "no-cache" }).then(r => r.json());
```

Or load the JS global directly:

```html
<script src="https://raw.githubusercontent.com/jmacAJ/lanacup-data/main/js/lanacup_data.js"></script>
<script>
  console.log(window.LANACUP_DATA);
</script>
```

## Current snapshot

- Generated at: `2026-05-02T22:49:34.174945+00:00`
- Status: `official_2026_groups_fixtures_and_knockout_mapping_loaded`
- SHA-256: `0b94b713e9c5e8b79e89845fa9d5681e6010ca63a4cf727a0aa4720341b97f94`
