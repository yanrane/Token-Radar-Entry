# Token Radar

A market-priced board of 200 pre-token protocols, ranked by what a token launch would be worth.

The model asks the market instead of guessing: the multiple is the median market cap per dollar of TVL
among live-token protocols in the same category (128 live tokens on this snapshot; whole-market median
0.2138, Dexs 0.3424 over 11 comparables, CDP 0.1687 over 3). Every row carries the multiple it used and
its sample size, so a reader can check the claim against the snapshot.

## What it covers

- 200 rows: all 40 watchlist protocols plus 160 earlier pre-token protocols below the floor
- Each row carries 3-12 concrete farm steps with a cost and a time
- Static dashboard: the board, a per-protocol detail view, and a filter. No framework, no network.

## Run

    node --experimental-strip-types main.ts --input /input/snapshot.json --output /output

Two runs over the same snapshot write byte-identical files.

## Licence

MIT. See LICENSE.
