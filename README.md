# Sebastian Cordoba

MSc Mathematics & Finance @ Imperial College London. I work on quantitative research and systematic trading — mostly machine learning applied to derivatives, market microstructure, and time-series forecasting.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/sebastian-cordoba-topete-622960271)
[![Email](https://img.shields.io/badge/Email-sebastian.cordobat%40proton.me-red)](mailto:sebastian.cordobat@proton.me)

## About

I'm finishing an MSc in Mathematics and Finance at Imperial (Ramón Areces Foundation full scholarship), after a First Class Honours degree in Mathematics from Aberdeen (85%). Before Imperial I spent two years building AI patent classifiers at LexisNexis and a year as a quant analyst in Madrid.

Living through the 2008 crisis is what got me into this!

Right now I trade and research for **Team Delta / QTC Alpha Fund** at Imperial.

## Featured projects

### Replicating a signature-transform forecaster — [signature-transform-replication](https://github.com/tessella/signature-transform-replication)
A from-scratch replication of [Gu et al. (2025)](https://doi.org/10.1287/inte.2023.0067), an Adaptive Two-Step LASSO that weights history by signature-kernel distance. I found the published algorithm quietly degenerates to a last-value predictor (an anchor self-matching bug), and carries a lookahead-bias flaw that I fixed with expanding-window normalisation. The best honest result is **0.75% MAPE** at 12 weeks against a **1.02%** naive carry-forward baseline — the paper's claimed 0.31% was not reproducible from the public feature set.

### High-frequency price-movement prediction — [High-frequency-price-movement-prediction](https://github.com/tessella/High-frequency-price-movement-prediction)
A deep-learning classifier for limit-order-book data. I engineered features from 4-level depth (bid/ask volumes, imbalances, pressures) and compared feedforward vs. recurrent architectures, reaching **71.3%** validation accuracy in TensorFlow/Keras.

### UK gas-demand forecasting — [UK-Gas-Demand-Forecasting](https://github.com/tessella/UK-Gas-Demand-Forecasting)
Gradient-boosted regression where most of the work was domain feature engineering. I built a custom windchill index to turn raw weather into a demand signal, getting to **R² = 0.951**.

### A neural network in C — [xor-problem-nn-c](https://github.com/tessella/xor-problem-nn-c)
A feedforward net written in plain C, no ML libraries: manual memory management, gradient descent and the cost function from the ground up.

### C++ exam solutions — [cpp-exam-prep](https://github.com/tessella/cpp-exam-prep)
Self-contained single-file solutions to past papers from Imperial's Computing in C++ module: templates, RAII, polymorphism, and the numerical-methods staples (root-finding, LU decomposition, Monte Carlo).

## Tools

**Languages**: Python, C++, C

**Python**: PyTorch, TensorFlow/Keras, scikit-learn, XGBoost, LightGBM, pandas, NumPy, SciPy

**Finance**: options pricing, market microstructure, time-series forecasting, Monte Carlo methods, broker/data APIs

## Experience

**Quantitative Trader & Researcher** — Team Delta, QTC Alpha Fund, Imperial College (current)

**Solutions Analyst** — LexisNexis, London (2023–2025)
Led patent-intelligence delivery for Fortune 500 tech and defence clients, ran classifier projects of 10–40+ components, and was technical lead on a £1M+ portfolio across three accounts. Built AI classifiers over a 70M+ patent database, including work with Google DeepMind on technology identification.

**Quantitative Investment Analyst** — SafeBrok Europe, Madrid (2022)
Contributed to 20% fund growth through a downturn, and automated investment screening via a Python–Morningstar pipeline.

## Education

**Imperial College London** — MSc Mathematics and Finance (2025–2026)
Ramón Areces Foundation Scholar. Focus: machine learning, derivatives pricing, systematic trading, optimisation.

**University of Aberdeen** — BSc (Hons) Mathematics (2019–2023)
First Class Honours, 85%. Dissertation on smooth manifolds and polynomial vector fields on spheres.

## Contact

- Email: sebastian.cordobat@proton.me
- LinkedIn: [sebastian-cordoba-topete](https://www.linkedin.com/in/sebastian-cordoba-topete-622960271/)
- Based in London. Work permits (no visa needed): UK, USA, EU.

Open to roles in quantitative trading, market making, and quantitative research.
