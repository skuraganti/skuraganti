# Sashank Kuraganti

Independent projects in software, data engineering and AI, built around practical workflows and inspectable evidence.

The links below open interactive browser demonstrations. Each repository also contains the full Python/Docker application, architecture notes, reproducible data preparation and verification records. Hosted demos use labeled synthetic fixtures, captured data or recorded results. Backend workers run locally; optional model calls use a configured host bridge and may use remote inference.

## Start here

- **[Relay](https://github.com/skuraganti/data-pipeline-monitor):** follow a quarantined source row, inspect checkpoint recovery and see why only a complete normal run publishes a report.
- **[Folio](https://github.com/skuraganti/private-ai-knowledge-engine):** compare retrieval approaches and inspect exact supporting pages. The small held-out study includes a lexical baseline, abstentions and failures.
- **[Contour](https://github.com/skuraganti/ai-codebase-explorer):** explore source-linked symbols and import paths, then trace potential consumers of a changed module. Static reachability is qualified as potential impact.

## All projects

| Project | Explore | Engineering focus | Roadmap |
|---|---|---|---|
| **Ledger** | [Demo](https://skuraganti.github.io/personal-spending-tracker/) · [Code](https://github.com/skuraganti/personal-spending-tracker) | Transaction imports, category rules, recurring-payment candidates and budgets. | [Board](https://github.com/users/skuraganti/projects/1) |
| **Fieldglass** | [Demo](https://skuraganti.github.io/live-earth-dashboard/) · [Code](https://github.com/skuraganti/live-earth-dashboard) | Earthquake and weather ingestion, map playback and location watches. | [Board](https://github.com/users/skuraganti/projects/2) |
| **Relay** | [Demo](https://skuraganti.github.io/data-pipeline-monitor/) · [Code](https://github.com/skuraganti/data-pipeline-monitor) | Scheduled ingestion, quality checks, lineage and recoverable processing. | [Board](https://github.com/users/skuraganti/projects/3) |
| **Folio** | [Demo](https://skuraganti.github.io/private-ai-knowledge-engine/) · [Code](https://github.com/skuraganti/private-ai-knowledge-engine) | Document ingestion, hybrid retrieval, cited answers and deletion propagation. | [Board](https://github.com/users/skuraganti/projects/4) |
| **Contour** | [Demo](https://skuraganti.github.io/ai-codebase-explorer/) · [Code](https://github.com/skuraganti/ai-codebase-explorer) | Python/TypeScript indexing, dependency graphs and change-impact analysis. | [Board](https://github.com/users/skuraganti/projects/5) |
| **TraceLab** | [Demo](https://skuraganti.github.io/ai-agent-evaluation-lab/) · [Code](https://github.com/skuraganti/ai-agent-evaluation-lab) | Tool-planning benchmarks, immutable traces, replay and injection tests. | [Board](https://github.com/users/skuraganti/projects/6) |
| **Faultline** | [Demo](https://skuraganti.github.io/ai-incident-investigator/) · [Code](https://github.com/skuraganti/ai-incident-investigator) | Correlated logs, metrics and traces with evidence-linked diagnoses. | [Board](https://github.com/users/skuraganti/projects/7) |

## Screenshots

These previews are captured from the public browser demos. Expand a project to inspect its interface and data mode.

<details>
<summary>Ledger — preview</summary>

Synthetic GBP fixture; CSV processing stays in the browser.

<img src="assets/personal-spending-tracker.png" alt="Ledger: synthetic GBP spending, budget controls and recurring-charge candidates." width="1100" />

[Try the demo](https://skuraganti.github.io/personal-spending-tracker/) · [Read the source](https://github.com/skuraganti/personal-spending-tracker)

</details>

<details>
<summary>Fieldglass — preview</summary>

Captured USGS/NWS observations; the hosted demo does not poll live feeds.

<img src="assets/live-earth-dashboard.png" alt="Fieldglass: captured earthquake observations, magnitude filtering and event-time map playback." width="1100" />

[Try the demo](https://skuraganti.github.io/live-earth-dashboard/) · [Read the source](https://github.com/skuraganti/live-earth-dashboard)

</details>

<details>
<summary>Relay — preview</summary>

Actual NYC TLC aggregates with explicitly simulated browser queue/retry behavior.

<img src="assets/data-pipeline-monitor.png" alt="Relay: real taxi-data quality aggregates and simulated queue and retry controls." width="1100" />

[Try the demo](https://skuraganti.github.io/data-pipeline-monitor/) · [Read the source](https://github.com/skuraganti/data-pipeline-monitor)

</details>

<details>
<summary>Folio — preview</summary>

Lexical search and extractive citations over captured NIST document passages.

<img src="assets/private-ai-knowledge-engine.png" alt="Folio: lexical search and extractive citations from captured NIST document passages." width="1100" />

[Try the demo](https://skuraganti.github.io/private-ai-knowledge-engine/) · [Read the source](https://github.com/skuraganti/private-ai-knowledge-engine)

</details>

<details>
<summary>Contour — preview</summary>

Saved parser output from pinned Flask/Zod source; no analyzed code is executed.

<img src="assets/ai-codebase-explorer.png" alt="Contour: saved architecture map and static imports from pinned Flask and Zod source." width="1100" />

[Try the demo](https://skuraganti.github.io/ai-codebase-explorer/) · [Read the source](https://github.com/skuraganti/ai-codebase-explorer)

</details>

<details>
<summary>TraceLab — preview</summary>

Recorded BFCL-derived planning results; tool receipts and faults are simulated.

<img src="assets/ai-agent-evaluation-lab.png" alt="TraceLab: labeled synthetic sorting probe, policy selection and declared tool schema." width="1100" />

[Try the demo](https://skuraganti.github.io/ai-agent-evaluation-lab/) · [Read the source](https://github.com/skuraganti/ai-agent-evaluation-lab)

</details>

<details>
<summary>Faultline — preview</summary>

Measured sandbox telemetry with injected causes and saved diagnoses; no repair executor.

<img src="assets/ai-incident-investigator.png" alt="Faultline: measured HTTP failures, correlated request traces and a qualified study readout." width="1100" />

[Try the demo](https://skuraganti.github.io/ai-incident-investigator/) · [Read the source](https://github.com/skuraganti/ai-incident-investigator)

</details>

## What to inspect

- **Data provenance:** publisher links, acquisition scripts, sampling, licenses and limitations in each `DATA_SOURCES.md`.
- **Engineering decisions:** architecture, alternatives and tradeoffs in `ARCHITECTURE.md` and `DECISIONS.md`.
- **Verification:** domain tests, browser checks, persistence/recovery checks and recorded evaluation limits in `VERIFICATION.md`.
- **AI evaluation:** baselines, held-out questions or benchmark tasks, source citations and retained failures in the relevant repositories. Results are scoped to the documented samples.

## Running the full applications

Each project has its own dependencies, configuration, Docker Compose setup and data storage. Start with its README, run one stack at a time on a small machine, and use the documented local URL. GitHub Pages does not run the Python services or model bridges.

## Technologies and engineering

Python, SQL and browser JavaScript support the applications, with Docker Compose for isolated local services. Each project documents its architecture, dependency locks, data preparation, domain tests and browser checks. Recovery tests, source-linked analysis and bounded evaluation studies make the results inspectable.
