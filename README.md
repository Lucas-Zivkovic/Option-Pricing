# 🧮 OptionPricer – Monte Carlo & Analytical Option Pricing

## 🎯 Project Overview
This project implements, compares, and visualizes different **financial option pricing methods** under the **Black–Scholes model**, using both analytical formulas and numerical simulations (Monte Carlo).  
It demonstrates fundamental concepts in quantitative finance and stochastic simulation.

The notebook explores pricing and hedging (delta hedging) for several option types:
- ✅ **European Call**
- ✅ **Digital (cash-or-nothing)**
- ✅ **Asian**
- ✅ **Lookback**
- ✅ **Barrier options (up-and-out / down-and-in)**

---

## 🧠 Key Concepts
- Geometric Brownian Motion (GBM) model
- Risk-neutral pricing
- Monte Carlo approximation
- Analytical vs numerical comparison
- Greeks calculation (Δ)
- Variance reduction and Monte Carlo convergence
- Error analysis and visualizations (delta, convergence)

---

## ⚙️ Repository Structure
```
OptionPricer/
│
├── OptionPricer.ipynb      # Main notebook: implementation & visualizations
├── requirements.txt        # Required libraries
└── README.md              # This file
```

---

## 🚀 Installation & Execution

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Lucas-Zivkovic/Option-Pricing.git
cd OptionPricer
```

### 2️⃣ Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3️⃣ Install dependencies
```bash
pip install -r requirements.txt
```

### 4️⃣ Launch the notebook
```bash
jupyter notebook OptionPricer.ipynb
```

---

## 🧩 Main Libraries
- **numpy, math** – numerical computation
- **scipy.stats** – cumulative distribution functions (normal, etc.)
- **torch** – GPU-accelerated simulation
- **matplotlib** – visualizations

---

## 📊 Key Results
The notebook demonstrates:
- Monte Carlo convergence toward analytical Black–Scholes formulas
- Delta evolution and its impact on hedging strategies
- Behavior of exotic products (Asian, Barrier, Lookback)


---

## 🧱 Code Architecture
The code is organized around modular functions:

- `BlackScholesCallPricing()` — analytical BS formula
- `MonteCarlosEuCallOption()` — Monte Carlo simulation for European call
- `MonteCarlosDigitalOption()`, `MonteCarlosBarrierOption()` — exotic variants
- `HedgePortfolioDigit()` — delta hedging strategy simulation

- `Etc`

Each function includes:
- Standard financial parameters (S0, K, T, σ, r, N)
- Documentation
- Input validation
- CPU/GPU execution support (torch)


---

## 👤 Author
**Lucas Živković**  
Master's student in Finance, Applied Mathematics & Computer Science  
Passionate about quantitative finance, numerical simulation, and machine learning applied to financial markets.

📧 lucas.zivkovic0@gmail.com  
🔗 [LinkedIn](https://linkedin.com/in/lucas-zivkovic) | [GitHub](https://github.com/Lucas-Zivkovic)

---

## 📜 License
This project is released under the MIT License – free to use and modify.