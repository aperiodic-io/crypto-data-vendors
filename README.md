# Crypto market data vendors compared

A side-by-side comparison of crypto market data vendors on 40 criteria: coverage, history, timestamps, raw data types, derived metrics, delivery, pricing and access. Every fact comes from the vendor's own public pages and carries the date it was checked.

**Browse it at [aperiodic.io/compare](https://aperiodic.io/compare).** The website is the reference version. It has filters, a page per vendor, every source behind every cell, and the change log. This repository holds the same data as files.

> [!IMPORTANT]
> **Built by Aperiodic, which is one of the columns, so this is not an independent review.** Nobody is ranked, Aperiodic included. Facts come from each vendor's own public pages, with the date they were checked. Rows marked "Our judgement" are opinion. Corrections: [info@aperiodic.io](mailto:info@aperiodic.io).

## Where to find it

| | |
|---|---|
| **Website (reference)** | [aperiodic.io/compare](https://aperiodic.io/compare) |
| How it is compiled | [aperiodic.io/compare/methodology](https://aperiodic.io/compare/methodology) |
| Data in this repository | [`data/crypto-data-vendors.csv`](data/crypto-data-vendors.csv), [`data/crypto-data-vendors.json`](data/crypto-data-vendors.json) |
| Google Sheet | [View the sheet](https://docs.google.com/spreadsheets/d/1Z_BvjLlfMSTbOd7qVApVsnM4cVWzWwKDo9cp1WLUHAg/edit?usp=sharing) |

The Google Sheet is where the comparison was first compiled, and it stays open for reading. The website and the files here are stricter. When a value has no vendor page behind it, they show it as Not verified instead. If the sheet and the website disagree, go by the website.

## What it covers

18 columns:

- **Raw market data:** Tardis.dev, CoinAPI, Kaiko, Crypto Lake, CoinDesk Data, and the exchanges' own free archives
- **Derived market metrics:** Aperiodic.io, Amberdata, Coin Metrics
- **Derivatives analytics:** Velo, Laevitas, CoinGlass, Coinalyze, Hyblock Capital
- **On-chain analytics:** glassnode, CryptoQuant
- **Reference data:** CoinGecko, CoinMarketCap

This is a selection of the vendors researchers name when they shop for crypto market data, not a complete list.

40 criteria in five sections:

1. **What it is:** primary product, ownership
2. **Universe and integrity:** exchanges covered, full instrument universe, delisted instruments, earliest data, history by plan, local timestamps, aggregation ordering, restatements
3. **What you get:** tick trades, L2 updates and snapshots, L3, options, and derived metrics such as bars, order flow, trade size, market impact, slippage, realized volatility, L1 and L2 depth, and derivatives
4. **Access and commercials:** delivery format, rate limits, backfill friction, pricing model, what the price gates, full history on a monthly subscription, entry price, keyless access, self-serve signup
5. **In one line:** best suited to, main gotchas (our judgement, labelled as such)

## How to read a cell

| Status | Meaning |
|---|---|
| Yes | Stated in the vendor's own public documentation. |
| Partial | True with a caveat, spelled out in the cell. |
| No | Not offered, per the vendor's own documentation. A No is not a criticism: it can be the right call for what the product is. |
| n/a | The question does not apply to this kind of product. |
| Documented | A value from the vendor's own public pages. |
| Vendor claim | A marketing figure we could not check independently. |
| Not verified | We could not confirm it either way. Do not read it as a No. |
| Not documented | We read the vendor's own docs and they do not say. Ask the vendor. |
| Not disclosed | The vendor's own pages do not name who operates it. |
| Our judgement | Opinion, labelled as such. Not a documented fact. |

## The files

**`data/crypto-data-vendors.csv`** has one row per cell (18 vendors × 40 criteria). GitHub shows it as a searchable table.

| Column | Contents |
|---|---|
| `vendor_id`, `vendor` | The column |
| `section`, `criterion_id`, `criterion` | The row |
| `status` | One of the statuses above |
| `value` | What the vendor's pages say |
| `note` | Extra context, where there is any |
| `source_urls` | The vendor pages the value comes from, space-separated |
| `checked` | The date those pages were last checked |

**`data/crypto-data-vendors.json`** holds the whole comparison: vendors, sections, criteria (with what each one asks), every source with its URLs and check date, every cell, the status legend, and the change log. `updated` is the date of the latest change.

## How it stays current

Each week an automated re-check reads the vendor pages whose cells are due and proposes changes as a pull request. Every change carries its source and date, and a person reviews it before anything goes live. Plan, price and ownership rows are due every 4 weeks, everything else every 12. The re-check never edits Aperiodic's own column.

This repository copies the published data from aperiodic.io every day ([`.github/workflows/sync.yml`](.github/workflows/sync.yml)), so the files match the website.

## Corrections

Products and prices change, and we may have misread something. If a cell is wrong, email [info@aperiodic.io](mailto:info@aperiodic.io) or [open an issue](https://github.com/aperiodic-io/crypto-data-vendors/issues) with the cell and the vendor page that shows the right answer. That goes for cells wrong in our favour as much as ones wrong against anyone else. If you work at one of these companies, the same address reaches us.

## Reuse

© 2026 Aperiodic Limited. You may quote individual cells or short excerpts, with a link to [aperiodic.io/compare](https://aperiodic.io/compare) and a note that Aperiodic built it, and use the downloads for your own research. Republishing the table, or a substantial part of it, needs our written permission: [info@aperiodic.io](mailto:info@aperiodic.io). See [LICENSE](LICENSE).

The facts themselves come from the vendors' own pages, and their names and trademarks belong to them.
