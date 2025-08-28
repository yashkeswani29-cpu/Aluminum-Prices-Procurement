# Aluminum Price Volatility Forecasting & Hedging for Breweries

This project applies **econometric (GARCH)** and **AI (LSTM)** models to forecast aluminum price volatility and design a **hedging strategy** for breweries that depend on aluminum cans.  
It transforms procurement from reactive buying into a **predictive, data-driven risk management framework**.

---

## 🚀 Key Objectives
- Forecast aluminum futures volatility using:
  - **GARCH(1,1)-t** (traditional econometric model)
  - **LSTM neural network** (deep learning model)
- Evaluate models with **MSE, MAE, QLIKE**.
- Translate forecasts into **hedge ratios** for breweries.
- Compute hedge needs in **LME futures contracts (25-ton lots)**.
- Compare GARCH vs LSTM hedging recommendations.

---

## 📊 Workflow
1. **Data Collection**  
   - Aluminum futures data (`ALI=F`) fetched from Yahoo Finance.  
   - Daily returns and realized volatility (squared returns) computed.  

2. **Modeling**  
   - **GARCH(1,1)-t**: captures volatility clustering, conservative, reacts to spikes.  
   - **LSTM**: uses 21-day lookback to predict next-day volatility, smoother and cost-efficient.  

3. **Evaluation**  
   - Metrics: **MSE, MAE, QLIKE**.  
   - Visualization of actual vs forecasted volatility.  

4. **Hedging Strategy**  
   - Minimum-variance hedge ratio computed.  
   - Hedge recommendations converted into **25-ton futures lots**.  
   - Comparison:  
     - GARCH → more frequent adjustments, higher protection, higher cost.  
     - LSTM → steadier hedging, lower costs, higher exposure risk.  
   - Hybrid approach recommended. 

