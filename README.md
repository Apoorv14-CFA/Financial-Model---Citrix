# Financial-Model---Citrix
Private-company DCF valuation of Citrix Systems (pre/post its 2022 Vista Equity/Elliott LBO) — built from scratch in Excel, fully sourced to 10-Ks and merger filings. Covers comps-based WACC, LBO capital structure, GAAP-to-Non-GAAP reconciliation, and DCF vs. actual deal price comparison.
# Citrix Systems — Private Company DCF Model

A fully sourced discounted cash flow valuation of Citrix Systems, built as a private-company case study around its 2022 take-private by Vista Equity Partners and Elliott Management ($16.5B LBO).

## Why this case
Citrix went private in September 2022, which means no stock price, no market beta, and no market cap to lean on — the standard public-company DCF toolkit doesn't apply. This model uses the private-company valuation methodology instead: unlevering comparable public companies' betas, relevering onto Citrix's actual post-LBO capital structure, and cross-checking every historical figure against real 10-K filings.

## Model structure
- **Revenue Build** — driver-based forecasting across 4 revenue lines (SaaS, Non-SaaS Subscription, Product & License, Support & Services), explicitly accounting for Citrix's 2020 structural shift away from perpetual licensing
- **Operating Expense Build** — bottom-up margin build, reconciled against a GAAP-to-Non-GAAP bridge and Citrix's own guidance
- **D&A and Capex Schedule** — sourced from cash flow statements, with Citrix's own disclosed forward amortization schedule
- **Net Working Capital** — models the cash-flow benefit of Citrix's subscription/deferred-revenue model
- **WACC** — comps-based unlevered beta (Cisco, F5, Microsoft), relevered onto Citrix's actual disclosed LBO debt structure (sourced from merger proxy filings)
- **Unlevered FCF & DCF** — full 5-year explicit forecast, terminal value, sensitivity table, and an Enterprise Value → Equity Value bridge
- **Deal comparison** — DCF-implied equity value benchmarked against the actual $13.06B price paid by Vista/Elliott

## Key results
| Metric | Value |
|---|---|
| WACC | 8.4% |
| Enterprise Value | $12.7B |
| Implied Equity Value | $9.9B |
| Actual deal equity value (Jan 2022) | $13.1B |
| Implied discount vs. actual deal | ~24% |

## Sourcing
Every hardcoded input is tagged to its source — Citrix's FY2019-2021 10-Ks, cash flow statements, merger proxy filings (DEFM14A/PREM14A), and comparable companies' balance sheets. See `Assumptions_Defense_Guide.docx` for the full rationale and sourcing behind every assumption.

## Formatting convention
Follows FAST-standard color coding: **blue** = hardcoded input, **black** = same-sheet formula, **green** = cross-sheet link, **red** = validation check.

## Files
- `Citrix_DCF_Model.xlsx` — the full model
- `Citrix_Model_Assumptions_Defense_Guide.docx` — assumption-by-assumption sourcing and rationale
