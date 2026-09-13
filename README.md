# bybit-linear

> bybit · linear · paper

[![Python 3.11+](https://img.shields.io/badge/python-3.11+-3776AB)](https://python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Build](https://img.shields.io/badge/build-passing-brightgreen)]()

Bybit linear paper bot — grid strategy id.

## Features

- Default venue bybit / BTCUSDT
- Built-in grid strategy plus paper mode
- Risk manager with daily-loss kill switch
- OHLCV store and SHA-256 stub candles
- Backtester with fill + fee model
- Click CLI: backtest, paper, status, orders

## Prerequisites

- Python 3.11+
- Git

## Getting Started

```bash
git clone <repo-url>
cd bybit-linear
python -m pip install -e .
python -m bybitlin --help
```

## CLI Usage

```bash
bybitlin backtest --bars 200
# Replay stub candles

bybitlin paper
# Start a paper session

bybitlin status
# Print engine state

bybitlin orders
# List simulated fills
```

## Project Structure

```
bybitlin/
  core/        engine + risk
  strategy/    grid / dca / ema hooks
  exchange/    stub order client
  data/        candles + backtest
  cli.py
tests/
```

## Configuration

See `bybitlin/config.py`.

| Setting | Default | Description |
|---------|---------|-------------|
| `exchange` | `bybit` | Venue id |
| `symbol` | `BTCUSDT` | Default pair |
| `strategy` | `grid` | Active strategy |
| `mode` | `paper` | paper or backtest |

## Tests

```bash
python -m pytest -q
```

## Background

Bybit API threads start from bybit-linear.

## License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.


---

## Topics

![bybit](https://img.shields.io/badge/bybit-111827?style=flat-square) ![linear](https://img.shields.io/badge/linear-111827?style=flat-square) ![bybit-linear](https://img.shields.io/badge/bybit%20linear-111827?style=flat-square) ![trading-bot](https://img.shields.io/badge/trading%20bot-111827?style=flat-square) ![crypto-trading](https://img.shields.io/badge/crypto%20trading-111827?style=flat-square) ![binance](https://img.shields.io/badge/binance-111827?style=flat-square) ![defi](https://img.shields.io/badge/defi-111827?style=flat-square) ![algorithmic-trading](https://img.shields.io/badge/algorithmic%20trading-111827?style=flat-square)

`bybit` `linear` `bybit-linear` `trading-bot` `crypto-trading` `binance` `defi` `algorithmic-trading` `quantitative-finance` `open-source` `python`

Search: bybit-linear · bybit · linear · paper · Bybit linear paper bot — grid strategy id.

---

<sub>Bybit linear paper bot — grid strategy id.</sub>
