# api-specs

Reverse-engineered OpenAPI specifications for services that do not publish official machine-readable specs. These files are referenced from the [rote adapter catalog](https://github.com/modiqo/rote/blob/main/src/adapters/catalog/catalog.csv).

## Contents

### polymarket/

| File | Description |
|---|---|
| `clob-api.openapi.json` | Central Limit Order Book API — orderbook data, pricing, order placement and cancellation |
| `data-api.openapi.json` | Data API — user positions, trades, activity, leaderboards, builder analytics (no auth required) |
| `gamma-api.openapi.json` | Gamma API — markets, events, tags, search, public profiles (no auth required) |

### rippling/

| File | Description |
|---|---|
| `api_spec_2024-08-01_API_Tier_1.yaml` | Rippling Platform API Tier 1 — HR, payroll, workforce management endpoints |

## Usage

Raw GitHub URLs for these specs are referenced directly in the rote adapter catalog and can be used with `rote adapter new`:

```bash
rote adapter new polymarket-clob https://raw.githubusercontent.com/modiqo/api-specs/main/polymarket/clob-api.openapi.json
rote adapter new polymarket-data https://raw.githubusercontent.com/modiqo/api-specs/main/polymarket/data-api.openapi.json
rote adapter new polymarket-gamma https://raw.githubusercontent.com/modiqo/api-specs/main/polymarket/gamma-api.openapi.json
rote adapter new rippling https://raw.githubusercontent.com/modiqo/api-specs/main/rippling/api_spec_2024-08-01_API_Tier_1.yaml
```
