# Evaluating Prediction Market Efficiency:  
## Can Statistical Models Outperform Kalshi-Implied Probabilities?

### Project Overview

Under the Efficient Market Hypothesis (EMH), market prices should represent the best available forecast given all publicly available information. However, in practice, prediction markets may deviate from efficiency due to factors such as low liquidity, heterogeneous participant skill, behavioural biases, and capital constraints.

This project investigates whether **statistical forecasting models can systematically outperform the probabilities implied by Kalshi prediction markets**, with a particular focus on **Stock price predictions**.

Rather than attempting to trade aggressively, the goal of this analysis is to evaluate **forecast accuracy, calibration, and economic significance**, and to understand the structural conditions under which prediction markets may exhibit persistent mispricing.

---

### Research Questions

This project is structured around the following core questions:

1. **Are Kalshi market prices well-calibrated estimators of true event probabilities?**
2. **Can a data-driven model produce probability estimates that are more accurate or better calibrated than the market?**
3. **Does any observed edge vary with market characteristics such as liquidity, contract type, or time to expiry?**
4. **If differences exist, are they economically meaningful after accounting for transaction costs and uncertainty?**

---

### Motivation

From a finance perspective, this problem closely parallels classic questions in:
- Market efficiency
- Asset mispricing
- Risk-neutral vs subjective probabilities
- Limits to arbitrage

From a data science perspective, it presents a practical forecasting challenge involving:
- Noisy, sparse, and imbalanced data
- Probabilistic prediction rather than point estimation
- Model calibration and uncertainty quantification
- Benchmarking against a strong baseline (the market itself)

Importantly, the Kalshi market price serves as a **natural benchmark**, analogous to using an index in asset pricing or implied volatility in options markets. Any model that fails to outperform this benchmark lacks practical relevance.

---

### Methodological Approach

The analysis proceeds as follows:

1. **Data Collection**
   - Historical Kalshi contract prices and settlement outcomes
   - Relevant public data sources associated with each event type

2. **Benchmark Construction**
   - Market-implied probabilities derived from contract prices
   - Evaluation of baseline accuracy and calibration

3. **Model Development**
   - Simple probabilistic baselines (e.g. historical frequencies)
   - Statistical and machine learning models where appropriate
   - Emphasis on interpretability and robustness

4. **Evaluation Framework**
   - Proper scoring rules (Brier score, log loss)
   - Calibration curves and reliability diagrams
   - Comparative performance against the market benchmark

5. **Economic Interpretation**
   - Identification of systematic biases
   - Discussion of market structure and limits to efficiency
   - Assessment of practical exploitability

---

### Scope and Limitations

This project does **not** claim to discover guaranteed trading profits or to refute market efficiency in general. Instead, it aims to provide a **careful, empirical evaluation** of whether prediction markets—particularly smaller or lower-attention markets—exhibit measurable inefficiencies that can be identified through disciplined statistical analysis.

Results are interpreted with caution, with particular attention paid to:
- Sample size limitations
- Overfitting risk
- Variance in short-horizon outcomes

---

### Relevance to Industry

This project mirrors real-world tasks performed in:
- Quantitative research
- Risk modelling
- Market research and forecasting
- Applied data science roles in finance and fintech

The emphasis on benchmarking, calibration, and decision-relevant interpretation reflects how probabilistic models are evaluated in professional settings, rather than academic toy problems.

---

### Repository Structure

