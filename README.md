# Hi, I'm Sebastián Córdoba 👋

MSc Mathematics & Finance @ Imperial College London | ML & Quantitative Research

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/sebastian-cordoba-topete-622960271)
[![Email](https://img.shields.io/badge/Email-sebastian.cordobat%40proton.me-red)](mailto:sebastian.cordobat@proton.me)

## About Me

Aspiring quantitative researcher passionate about applying rigorous mathematics and machine learning to financial markets. Currently pursuing an MSc in Mathematics and Finance at Imperial College London (funded by Fundación Ramón Areces scholarship), I combine a First Class Honours degree in Mathematics (85%) with hands-on experience in machine learning, financial modeling, and software development.

**What drives me**: Personal experience with the 2008 financial crisis shaped my commitment to developing more accurate quantitative models. I'm fascinated by markets at the intersection of mathematics, technology, and real-world impact.

## Current Work

**Quantitative Trader & Researcher** @ Team Delta, QTC Alpha Fund (Imperial College)

## Featured Projects

### UK Gas Demand Forecasting II: 

- **Core Method:** Adapted my own methodology (in turn adapted from [Transportation Marketplace Rate Forecast Using Signature Transform](https://pubsonline.informs.org/doi/10.1287/inte.2025.0251)) to model the physical dynamics of UK natural gas demand.
- **Implementation Challenges:** My original "local normalization" (Z-scoring) failed for gas forecasting, where absolute temperature levels drive demand. Additionally, the linear model could not capture the non-linearity of thermal efficiency in extreme cold.
- **Key Modifications:**
    - **Physics-Aware Normalization:** Replaced window-based scaling with global scaling to preserve absolute thermal signals (global scaling is acceptable for weather data as it is considered stationary).
    - **Global-Soft Weighting:** Pivoted to a globally-weighted Ridge Regression (Temperature $\approx$ 0.1) to utilize the full history while retaining soft regime-switching for structural breaks.
    - **Capturing Non-Linearity:** Computed level 3 signature on features to capture convexity in the data.
- **Results:** Achieved a **5.96% MAPE** (7-day ahead) and **7.92% MAPE** (14-day ahead), outperforming standard industry benchmarks [10%](https://www.mdpi.com/1996-1073/14/16/4905) and competing with commercial utility-grade models with a simple dataset.

### Paper Replication: [Transportation Marketplace Rate Forecast Using Signature Transform](https://pubsonline.informs.org/doi/10.1287/inte.2025.0251)

- **Core Method:** Replicates the authors' novel use of the signature transform (a "universal feature extractor") combined with an Adaptive Two-Step LASSO regression model
- **Implementation Challenges:** While the original paper utilized Amazon's proprietary dataset (100+ internal factors) to predict freight rates, replicating the methodology on public data (Consumer Loans) required significant algorithmic restructuring.
- **Key Modifications:** To achieve the authors' reported accuracy without their proprietary data infrastructure, the implementation required:
    - **Strict Local Normalization:** Replacing global scaling with window-based Z-scoring to eliminate lookahead bias while maintaining signal.
    - **Momentum-Based Targeting:** Shifting from predicting raw levels (which caused mean-reversion errors) to predicting normalized log-changes to capture directional trends.
    - **Autoregressive Signatures:** Augmenting the feature set with the signature of the target variable ($y$) itself, to capture momentum in the absence of internal signals.
    - **Robust Regularization:** Replacing auhtors' standard OLS refitting with `RidgeCV` to handle the extreme multicollinearity (condition numbers $>10^{16}$) inherent in signature features.
- **Results:** The modified model achieved a **1.07% MAPE** and **70.6% Directional Accuracy** on the validation set, reproducing the paper's claim of high-fidelity quarterly forecasting.

### High-Frequency Price Movement Prediction
Deep learning classifier for order book analysis achieving **71.29% validation accuracy**
- Feature engineering from 4-level limit order book data (bid/ask volumes, depth imbalances, concentration metrics)
- Compared feedforward vs. recurrent neural network architectures
- **Tech**: Python, TensorFlow/Keras, Pandas, NumPy

### UK Gas Demand Forecasting
Gradient boosting regression model with **R² = 0.951**
- Engineered windchill index combining temperature and wind data
- Demonstrated domain knowledge translation into predictive features
- **Tech**: Python, XGBoost, Sklearn, Feature Engineering

### Quantitative Risk Management
#### Tesla Risk Forecasting with EVT
ARCH Models & Extreme Value Theory
- Implemented GARCH(1,1) volatility modeling on Tesla returns
- Applied Extreme Value Theory with GPD for tail risk
- Compared Normal, Student-t, and GPD residual distributions
- Generated out-of-sample VaR & ES forecasts at 95% and 99% levels
- **Tech**: Python, ARCH, EVT, Risk Metrics, Backtesting, Statistical Testing
#### DOG ETF Risk Analysis</h3>
Comparative VaR & ES Forecasting   
- Historical Simulation with 500-day rolling window
- Filtered Historical Simulation with EWMA (α=0.06)
- FHS-GARCH(1,1) for dynamic volatility modeling
- FHS-EWMA achieved best performance across coverage tests
- **Tech**: Python, FHS, EWMA, ARCH, Statistical Testing, Backtesting

### Neural Networks from Scratch
Built complete feedforward network without ML libraries
- Gradient descent and cost function optimization implemented manually
- Developed thorough understanding of ML fundamentals
- **Tech**: C, Manual Memory Management, Core ML Algorithms

## Technical Stack

**Languages**: Python • C++ • C 

**Python Ecosystem**: 
- ML/DL: TensorFlow, Keras, PyTorch, Sklearn, XGBoost
- Data: Pandas, NumPy, SciPy
- Viz: Matplotlib, Seaborn, Plotly

**Finance & Trading**: Alpaca API • Market Microstructure • Options Pricing • Time Series Forecasting

**Mathematical Expertise**: Statistics • Probability • Differential Equations • Topology • Optimization • Monte Carlo Methods

## Professional Experience

**Solutions Analyst** @ LexisNexis, London (2023-2025)
- Led patent intelligence delivery for Fortune 500 tech and defense clients, managing complex classifier projects (10-40+ components) and coordinating cross-functional analyst teams of 3-4 members
- Managed £1M+ client portfolio as primary technical lead across three major accounts, overseeing scope definition, quality assurance, and stakeholder presentations with 100% on-time delivery
- Built AI classifiers for 70M+ patent database, working with clients including Google DeepMind on advanced technology identification (AI algorithms, manufacturing processes, pharmaceutical developments...)

**Quantitative Investment Analyst** @ SafeBrok Europe, Madrid (2022-2022)
- Contributed to **20% fund growth** during market downturn
- Automated investment screening via Python-Morningstar API integration
- Implemented original data pipeline for opportunity detection

## Education

**Imperial College London** | MSc Mathematics and Finance (2025-2026)
- Ramón Areces Foundation Scholar (full scholarship)
- Focus: Machine Learning, Derivatives Pricing, Systematic Trading, Optimisation

**University of Aberdeen** | BSc (Hons) Mathematics (2019-2023)
- First Class Honours, 4.0 GPA (85%)
- Dissertation: Smooth manifolds and polynomial vector fields on spheres

## Languages

**English** • **Spanish** (Fluent/Native) | **French** (Basic)

## Get in Touch

- 📧 Email: sebastian.cordobat@proton.me
- 💼 LinkedIn: [Connect with me](#) <!-- Add your LinkedIn URL -->
- 📍 Location: London, UK
- 🗺️ Work permits (no visa required): United Kingdom, USA, European Union
---

> "I'm driven to understand markets through mathematics and build systematic strategies that combine rigorous quantitative analysis with practical implementation."

**Open to opportunities in**: Quantitative Trading • Market Making • Energy Trading • Quantitative Research • Financial Engineering

![Profile Views](https://komarev.com/ghpvc/?username=tessella&color=blueviolet)
