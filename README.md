# Stock Prediction Filter

Real-time stock price prediction using Linear Predictive Coding (LPC). Applies DSP techniques to financial time series with an interactive GUI for parameter tuning.

## Features

- Real-time stock price simulation via Geometric Brownian Motion
- LPC-based predictive filtering with adjustable parameters
- Interactive GUI with sliders for LPC order, window size, and decay factor
- Live prediction success rate and performance metrics
- Frequency response and cepstral analysis utilities

## Setup

```bash
python3 -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python src/main.py
```

## Project Structure

```
src/
  main.py              # Entry point
  gui.py               # Interactive parameter controls
  plot.py              # Real-time plotting and LPC
  analysis.py          # LPC coefficient calculation
  stock_simulation.py  # GBM price simulation
  synthesis.py         # LPC signal synthesis
  utils.py             # Frequency response, cepstral analysis
docs/                  # DSP and GUI documentation
```

## Tech Stack

Python, NumPy, SciPy, Matplotlib, scikit-learn, yfinance
