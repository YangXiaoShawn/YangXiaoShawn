# Yang Xiao

**Applied Economics · Causal Inference · Quantitative Finance**

[![Personal Homepage](https://img.shields.io/badge/Portfolio-yangxiaoshawn.github.io-2458cc?style=flat-square)](https://yangxiaoshawn.github.io/)
[![Unified Monorepo](https://img.shields.io/badge/Monorepo-open--economic--quant-16243a?style=flat-square)](https://github.com/YangXiaoShawn/open-economic-quant)
[![Live Trading Monitor](https://img.shields.io/badge/Live_OOS_Monitor-Daily_Trading_Results-157366?style=flat-square)](https://yangxiaoshawn.github.io/#daily-monitor)
[![Hugging Face Dataset](https://img.shields.io/badge/HF_Dataset-4,042_Verified_Files-a34f18?style=flat-square)](https://huggingface.co/datasets/ShawnChamberlain/open-economic-quant-research-data)
[![Interactive Space](https://img.shields.io/badge/HF_Space-Evidence_Observatory-7151a3?style=flat-square)](https://huggingface.co/spaces/ShawnChamberlain/open-economic-quant-research-observatory)

I study how economic incentives, public policy, and information shape market outcomes. My work connects applied econometrics with quantitative asset pricing across a unified 8-project research monorepo ([`open-economic-quant`](https://github.com/YangXiaoShawn/open-economic-quant)) powered by `oeq-core v0.2.0` and tracked day by day in out-of-sample markets.

- **Personal Homepage & Interactive Portfolio:** [https://yangxiaoshawn.github.io/](https://yangxiaoshawn.github.io/)
- **Live Out-of-Sample Daily Trading Monitor:** [https://yangxiaoshawn.github.io/#daily-monitor](https://yangxiaoshawn.github.io/#daily-monitor)
- **Daily Report Archive & Updated Results:** [Daily Reports](https://yangxiaoshawn.github.io/daily-reports/) · [Updated Results](https://yangxiaoshawn.github.io/updated-results/)
- **Full Research Data & Interactive Lab:** [Hugging Face Dataset](https://huggingface.co/datasets/ShawnChamberlain/open-economic-quant-research-data) · [Hugging Face Space](https://huggingface.co/spaces/ShawnChamberlain/open-economic-quant-research-observatory)

---

## Unified Architecture (`open-economic-quant`)

All eight empirical systems share a centralized econometric and portfolio infrastructure (`oeq-core v0.2.0`) with automated CI verification (`verify_monorepo.py` & `sync_ecosystem.py`):

1. **Statistical & Econometric Primitives:** Empirical Bayes adaptive cross-sectional shrinkage, Ledoit-Wolf covariance regularization, Newey-West HAC inference, Politis-Romano stationary bootstrap, White Reality Check, and Deflated Sharpe Ratio (DSR).
2. **Execution & Implementation Shortfall:** Turnover-damped portfolio weights, break-even transaction cost solvers, latency-grid simulation, and Almgren-Chriss square-root market impact.
3. **Evidence Governance:** Explicit claim boundaries (`SYNTHETIC_SMOKE`, `OOS_PREDICTIVE_COMPARISON`, `BACKTEST_ASSOCIATION`, `CAUSAL_IDENTIFIED`) with automatic demotion when pre-trend or placebo gates fail.

---

## Eight Applied Economics & Quantitative Research Systems

| # | Study | Central Question | Key Finding | Links |
| :--- | :--- | :--- | :--- | :--- |
| **01** | **CasualLab**<br>*Experiments & Incentives* | Who should get the offer? | Complex CATE learners miss the known-truth recovery benchmark ($\text{RMSE } 0.0417$ vs $0.0247$ oracle); uniform allocation beats learned targeting under equal budgets. | [Study](https://yangxiaoshawn.github.io/projects/casuallab/) · [Repo](https://github.com/YangXiaoShawn/open-economic-quant-casuallab) |
| **02** | **Macroeconomics**<br>*Real-Time Forecasting* | Would the forecast work in real time? | Auditing $7,985$ feature cells shows that holding availability fixed while importing later revisions changes the GDP holdout ranking of all six forecasting models. | [Study](https://yangxiaoshawn.github.io/projects/macroeconomics/) · [Repo](https://github.com/YangXiaoShawn/open-economic-quant-macroeconomics) |
| **03** | **RealEstate**<br>*Housing & Household Finance* | Does a cheap mortgage keep a loan in place? | Each $+1\text{ pp}$ mortgage rate gap is associated with a $0.817$ conditional payoff hazard ratio ($18.3\%$ lower exit hazard) in a complementary log-log model. | [Study](https://yangxiaoshawn.github.io/projects/realestate/) · [Repo](https://github.com/YangXiaoShawn/open-economic-quant-realestate) |
| **04** | **TariffIncidence**<br>*Trade & Public Policy* | Who absorbed the tariff? | Pre-duty customs unit values stay near $+0.025$ log points across sample windows while duty-inclusive landed costs rise near $+0.15$, pointing to U.S. importer incidence. | [Study](https://yangxiaoshawn.github.io/projects/tariff-incidence/) · [Repo](https://github.com/YangXiaoShawn/open-economic-quant-tariff-incidence) |
| **05** | **Microstructure**<br>*Order Flow & Execution* | How much short-horizon edge does order flow carry? | Order-flow imbalance is gross-positive in $110 / 144$ latency scenarios (up to $+2.39\text{ bp}$), evaluated against a frozen $4.00\text{ bp}$ taker fee hurdle. | [Study](https://yangxiaoshawn.github.io/projects/microstructure/) · [Repo](https://github.com/YangXiaoShawn/open-economic-quant-microstructure) |
| **06** | **EMFactorTiming**<br>*Emerging-Market Equities* | Can machine learning time equity factors? | Across $801,536$ country-factor-months in 22 emerging markets, regional Empirical Bayes shrinkage ($+1.20\%\ R^2_{\text{OOS}}$, $1.91$ net Sharpe) beats high-turnover ML timing. | [Study](https://yangxiaoshawn.github.io/projects/em-factor-timing/) · [Repo](https://github.com/YangXiaoShawn/open-economic-quant-em-factor-timing) |
| **07** | **PolymarketFactors**<br>*Prediction Markets* | Which prediction-market signals survive a realistic backtest? | Removing five backtest artifacts across $4,000$ markets cuts naive 30d momentum IC eightfold ($-0.440 \to -0.054$); price-neutral illiquidity ($-0.072$), volatility ($-0.069$), and reversal ($-0.032$) survive. | [Study](https://yangxiaoshawn.github.io/projects/polymarket-factors/) · [Repo](https://github.com/YangXiaoShawn/open-economic-quant-polymarket-factors) |
| **08** | **CryptoFactors**<br>*Crypto Perpetuals* | Do equity microstructure factors travel to crypto? | Across $105$ coins over $730+$ days, low-price range ($+1.63$ Sharpe), funding carry ($+1.42$), and retail positioning ($+1.39$) transfer and power a live-tracked market-neutral deliverable. | [Study](https://yangxiaoshawn.github.io/projects/crypto-factors/) · [Repo](https://github.com/YangXiaoShawn/open-economic-quant-crypto-factors) |

---

## Live Out-of-Sample Daily Trading Monitor

Tracked daily on [yangxiaoshawn.github.io/#daily-monitor](https://yangxiaoshawn.github.io/#daily-monitor) with full implementation-shortfall stress audits:

- **CryptoFactors (`105` Perpetuals, Binance Vision + OKX UTC):**
  - **Product B Deliverable (24-Perp Short Hedge, 8h Funding & 1-Min Delay):** $+28.41\%$ cumulative net return ($+0.81$ Sharpe) over $537$ days ($500\text{k}\text{--}1\text{M}$ capacity), gaining $+1.52\%$ market-neutral alpha on the Oct 22 crash day.
  - **High-Volume Reversal (`REV_hi`, Wide-105):** $+8.35\%$ October 2026 MTD ($+10.50\%$ since Sep 1).
- **EMFactorTiming (`49` US-Listed Global/EM Style & Country ETFs):**
  - **Empirical Bayes Shrinkage Factor Tilt:** $+1.98\%$ 2026 YTD tradable ETF excess return (vs $-5.48\%$ `EEM`), with $517\text{--}1,720\text{ bp}$ break-even transaction cost.
  - **Conservative Investment (`IWD - IWF`):** $+5.99\%$ October 2026 MTD ($+5.05\%$ 2026 YTD), delivering $+3.09\%$ crisis alpha during the Oct 22 equity sell-off.
