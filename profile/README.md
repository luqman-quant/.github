<div align="center">

# luqman-quant

**Quantitative trading research — paper only**

*A one-person research organisation for building and, more often, rejecting trading strategies*

[![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)]()
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)]()
[![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)]()
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?logo=postgresql&logoColor=white)]()
[![Paper only](https://img.shields.io/badge/Trading-Paper_only-lightgrey)]()

**Designed, built and maintained by a solo developer**

</div>

---

## Owner

| | |
|---|---|
| **Name** | **Muhammad Luqman** |
| **Role** | Solo developer and researcher |
| **Scope** | Backtest harness, execution engine, research tooling, data pipeline, dashboard, infrastructure |
| **Location** | Terengganu, Malaysia |

---

## What this is

A personal research platform for algorithmic trading. It runs on **paper accounts only**.
Own capital, one owner, no product, no clients, no outside money.

The interesting part is not the trading. It is the harness around it — a system built on the
assumption that most strategies do not work, and that the hard engineering problem is proving
that honestly before any money is involved.

## How the work is organised

- **Pre-registration.** A strategy's rules, its market, its timeframe and the thresholds it must
  clear are written down and committed *before* the evaluation runs. The evidence is then held to
  what was registered, not to what looked good afterwards.
- **Walk-forward evaluation.** Out-of-sample windows, with warmup accounted for separately, so
  in-sample fitting cannot leak into the reported result.
- **Multiple-testing controls.** Testing many strategies against the same history produces winners
  by chance alone; the harness is built to say so rather than to hide it.
- **An evidence gate.** Promotion out of paper requires the registered gate to pass **and** a
  separate, manual decision by the owner. The system cannot promote itself.
- **Retirement is a result.** A rejected strategy is recorded with its verdict and kept, not
  quietly deleted. Negative results are the majority of the output and are treated as output.

## Engineering

Python 3.12 with `uv`, FastAPI, React, PostgreSQL, Docker. The repository carries its own
changelog, a lessons log written up whenever something surprised us, migration-versioned schemas,
and a test suite that gates every change.

---

## Notes

- **Repositories here are private.** This page is the public face of the organisation; the code,
  the strategies and the results are not published.
- **No strategy detail, no performance figures, and no results are published here** — by choice.
- **Nothing in this organisation is investment advice**, an offer, or a solicitation. It is a
  personal engineering and research project.

<div align="center">

*Built in the open about its method, closed about its positions.*

</div>
