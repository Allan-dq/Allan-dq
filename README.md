# Hi, I'm Qin (Allan) Dai 👋

Software engineer working across **AI / computer vision**, **backend systems** and **forecasting & quantitative modeling**.<br>
M.S. Applied Mathematics & Statistics, Johns Hopkins University · Los Angeles, CA

- **Now:** Software Engineer Intern at Newegg, where I build and run production computer-vision and warehouse automation services
- **Before:** credit research & risk analytics at Allianz Asset Management, data analytics at Allianz Partners, front-end engineering at Leroy Merlin China
- **Open source:** merged contributions to [QuantLib](https://github.com/lballabio/QuantLib) (C++ core and Python bindings), [statsmodels](https://github.com/statsmodels/statsmodels), [PyMC-Marketing](https://github.com/pymc-labs/pymc-marketing) and [cellpy](https://github.com/jepegit/cellpy); details [below](#open-source-contributions)

## Featured projects

| Project | What it does | Stack |
|---|---|---|
| [FreightLens AI](https://github.com/Allan-dq/freightlens-ai) · [live demo](https://huggingface.co/spaces/AllanDai/freightlens-ai) | Freight document and video verification. A pallet detector trained on real warehouse photos (0.55 AP50 on unseen sessions) runs in the browser; a LayoutLMv3 form model reaches 0.80 entity F1 on FUNSD | Python · PaddleOCR · LayoutLMv3 · YOLO · FastAPI |
| [Alphabet FP&A Forecast](https://github.com/Allan-dq/alphabet-fpa-forecast) · [exec summary](https://github.com/Allan-dq/alphabet-fpa-forecast/blob/main/reports/exec_summary.md) | Quarterly revenue and P&L forecast from 41 SEC XBRL filings, with a SQL reporting layer and variance bridges. Backtest WAPE 3.2%, vs 14.0% for seasonal naive and 4.0% for zero-shot TimesFM | Python · statsforecast · DuckDB · BigQuery |
| [OpenSync](https://github.com/Allan-dq/OpenSync) | Event-driven partner inventory sync (idempotency, outbox, retries/DLQ, LLM-assisted schema mapping). CI replays duplicates, stale versions and an outage → DLQ → replay on real PostgreSQL, Kafka and Redis | Java 21 · Spring Boot · Kafka · PostgreSQL · Redis |
| [Mortgage Prepayment Modeling](https://github.com/Allan-dq/mortgage-prepayment-modeling-freddie-mac) | Leakage-aware prepayment hazard on Freddie Mac loan-level data with calendar-time backtests. It drives a QuantLib Hull-White Monte Carlo MBS valuation (OAS, duration, convexity) on an illustrative pool | Python · scikit-learn · QuantLib |
| [CreatorKit AI](https://github.com/Allan-dq/CreatorKit-AI) | Seven schema-governed agents turn a design brief into a validated, token-compliant prototype; ships an MCP-compatible design-system tool server | TypeScript · React · Zod · Playwright |
| [Meridian MMM Case Study](https://github.com/Allan-dq/meridian-mmm-case-study) | Marketing-mix model on Google Meridian's simulated geo data, read out for finance: ROI vs marginal ROI with 90% credible intervals. The last 10% of the budget returns $0.61 per $1 | Python · Meridian · JAX |
| [Battery Cycling Data Pipeline](https://github.com/Allan-dq/battery-cycling-pipeline) | ETL, data-quality checks and anomaly detection on 119M rows of public battery-cycler data (169 cells). Reproduces the Severson 2019 early-cycle life model: RMSE 86 cycles (paper: 91) | Python · cellpy · DuckDB · MLflow · Docker |

**More projects:** [SoCal ZIP Market Score](https://github.com/Allan-dq/socal-zip-time-market-score) (0–100 ZIP-by-period market score, nested cross-validation) · [Thai Stock Market Chatbot](https://github.com/Allan-dq/News-Retrieval-of-Thailand-Stock-Market) (LLM Q&A with live SET data)

## Open-source contributions

- **[cellpy](https://github.com/jepegit/cellpy)** (battery-cycler data toolkit): [#1201](https://github.com/jepegit/cellpy/pull/1201), merged. The Neware `.nda`/`.ndax` loader now keeps the measured cell temperature and other auxiliary channels, which it used to drop; tested on the repository's own Neware fixture ([issue #1184](https://github.com/jepegit/cellpy/issues/1184)).
- **[QuantLib-SWIG](https://github.com/lballabio/QuantLib-SWIG)** (Python bindings for the QuantLib quant-finance library): [#955](https://github.com/lballabio/QuantLib-SWIG/pull/955), merged. Exposes the `NaturalCubicFitting` bond-curve fitting method to Python and adds the first Python tests for fitted bond discount curves.
- **[QuantLib](https://github.com/lballabio/QuantLib)** (C++ quant-finance library): [#3063](https://github.com/lballabio/QuantLib/pull/3063), merged. Adds the first tests for `NaturalCubicFitting` (evaluation, knot validation, calibration to bond prices) and fixes a bug they exposed: a negative knot time moved the d(0) = 1 constraint off t = 0, so the constructor now rejects it.
- **[statsmodels](https://github.com/statsmodels/statsmodels)** (statistics library for Python): [#10738](https://github.com/statsmodels/statsmodels/pull/10738), merged, ships in 0.15.1. Adds `krippendorff_alpha` to `stats.inter_rater`: agreement among any number of raters, with missing ratings, for nominal, ordinal, interval and ratio data. Results match the original paper and R.
- **[PyMC-Marketing](https://github.com/pymc-labs/pymc-marketing)** (Bayesian marketing-mix and customer-lifetime-value library): [#3347](https://github.com/pymc-labs/pymc-marketing/pull/3347), merged. HSGP recommendations now size the boundary `L` from the data's half-range, as `approx_hsgp_hyperparams` defines it, instead of its center; before, front-loaded time indexes could fall outside `[-L, L]`.

## Toolbox

- **Languages:** Python · Java · TypeScript · C# · C++ · SQL
- **ML & CV:** scikit-learn · OpenCV · YOLO · PaddleOCR · LayoutLMv3 · MLflow
- **Backend & infra:** FastAPI · Spring Boot · Kafka · PostgreSQL · Redis · Docker · Kubernetes
- **Quant & finance:** forecasting (statsforecast, hierarchical reconciliation) · FP&A modeling · marketing-mix modeling (Meridian) · SQL (DuckDB, BigQuery) · Data Studio dashboards · QuantLib (MBS/OAS, fitted bond curves) · credit risk · time-series validation
- **AI-assisted development:** ship with AI coding agents (Claude Code, MCP tooling) under test-gated review

## Contact

[LinkedIn](https://www.linkedin.com/in/qin-dai-817083347/) · allan.dai0921@gmail.com
