# Hi, I'm Qin (Allan) Dai 👋

Software engineer working across **AI / computer vision**, **backend systems** and **forecasting & quantitative modeling**.<br>
M.S. Applied Mathematics & Statistics, Johns Hopkins University · Los Angeles, CA

- **Now:** Software Engineer Intern at Newegg, where I build and run production computer-vision and warehouse automation services
- **Before:** credit research & risk analytics at Allianz Asset Management, data analytics at Allianz Partners, front-end engineering at Leroy Merlin China

## Featured projects

| Project | What it does | Stack |
|---|---|---|
| [FreightLens AI](https://github.com/Allan-dq/freightlens-ai) · [live demo](https://huggingface.co/spaces/AllanDai/freightlens-ai) | Freight document and video verification. Pallet detector trained on real warehouse photos (LOCO, 0.55 pallet AP50 on unseen sessions) runs in the browser; LayoutLMv3 form model (0.80 entity F1 on FUNSD) | Python · PaddleOCR · LayoutLMv3 · YOLO · ByteTrack · FastAPI |
| [Alphabet FP&A Forecast](https://github.com/Allan-dq/alphabet-fpa-forecast) · [exec summary](https://github.com/Allan-dq/alphabet-fpa-forecast/blob/main/reports/exec_summary.md) | Quarterly revenue and P&L forecast for Alphabet from 41 SEC XBRL filings, with a SQL reporting layer, variance bridges and scenarios. Backtest WAPE 3.2% on total revenue (seasonal naive 14.0%, zero-shot TimesFM 3.0 4.0%); 1.6% mean one-quarter-ahead revenue error over the last 8 quarters | Python · statsforecast · hierarchicalforecast · DuckDB · BigQuery |
| [OpenSync](https://github.com/Allan-dq/OpenSync) | Event-driven partner inventory sync with idempotency, out-of-order handling, transactional outbox, retries/DLQ and LLM-assisted schema mapping; CI runs an end-to-end test on real PostgreSQL, Kafka and Redis containers (duplicates, stale versions, outage → DLQ → replay) | Java 21 · Spring Boot · Kafka · PostgreSQL · Redis · OpenTelemetry |
| [Mortgage Prepayment Modeling](https://github.com/Allan-dq/mortgage-prepayment-modeling-freddie-mac) | Leakage-aware monthly prepayment hazard for Freddie Mac loan-level data, with calendar-time backtests and calibration; the model drives a QuantLib Hull-White Monte Carlo MBS valuation (OAS, effective duration and convexity) on an illustrative pool | Python · scikit-learn · QuantLib |
| [CreatorKit AI](https://github.com/Allan-dq/CreatorKit-AI) | Agentic design studio: seven schema-governed agents turn a brief into a validated, token-compliant prototype; ships an MCP-compatible design-system tool server | TypeScript · React · Zod · Storybook · Playwright |
| [Meridian MMM Case Study](https://github.com/Allan-dq/meridian-mmm-case-study) | Marketing-mix model built with Google Meridian on its simulated geo dataset, read out for finance: channel ROI vs marginal ROI with 90% credible intervals, a 10% budget reallocation, budget optimization and a budget-level test. Every channel's mean marginal ROI is below 1; the last 10% of the budget returns $0.61 of revenue per $1 | Python · Meridian · JAX · Bayesian MCMC |
| [Battery Cycling Data Pipeline](https://github.com/Allan-dq/battery-cycling-pipeline) | ETL, data-quality checks and anomaly detection on 119M rows of public battery-cycler time series (MATR/Severson 2019, NASA PCoE, 169 cells). Reproduces the paper's early-cycle life models: discharge model RMSE 86 cycles on the primary test (paper 91) | Python · cellpy · DuckDB · Parquet · MLflow · FastAPI · Docker |

**More projects:** [SoCal ZIP Market Score](https://github.com/Allan-dq/socal-zip-time-market-score) (0–100 ZIP-by-period market score, nested cross-validation) · [Thai Stock Market Chatbot](https://github.com/Allan-dq/News-Retrieval-of-Thailand-Stock-Market) (LLM Q&A with live SET data)

## Open-source contributions

- **[cellpy](https://github.com/jepegit/cellpy)** (battery-cycler data toolkit): [#1201](https://github.com/jepegit/cellpy/pull/1201), merged. The Neware `.nda`/`.ndax` loader now keeps the measured cell temperature and other auxiliary channels, which it used to drop; tested on the repository's own Neware fixture ([issue #1184](https://github.com/jepegit/cellpy/issues/1184)).
- **[QuantLib-SWIG](https://github.com/lballabio/QuantLib-SWIG)** (Python bindings for the QuantLib quant-finance library): [#955](https://github.com/lballabio/QuantLib-SWIG/pull/955), merged. Exposes the `NaturalCubicFitting` bond-curve fitting method to Python and adds the first Python tests for fitted bond discount curves.

## Toolbox

- **Languages:** Python · Java · TypeScript · C# · SQL
- **ML & CV:** scikit-learn · OpenCV · YOLO · PaddleOCR · LayoutLMv3 · MLflow
- **Backend & infra:** FastAPI · Spring Boot · Kafka · PostgreSQL · Redis · Docker · Kubernetes
- **Quant & finance:** forecasting (statsforecast, hierarchical reconciliation) · FP&A modeling · marketing-mix modeling (Meridian) · SQL (DuckDB, BigQuery) · Data Studio dashboards · QuantLib (MBS/OAS, fitted bond curves) · credit risk · time-series validation
- **AI-assisted development:** ship with AI coding agents (Claude Code, MCP tooling) under test-gated review

## Contact

[LinkedIn](https://www.linkedin.com/in/qin-dai-817083347/) · allan.dai0921@gmail.com
