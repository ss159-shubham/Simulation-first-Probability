# Module 6 — Gaussian Process, Aggregation & Risk Perception

## Overview

Module 6 extends the Bernoulli framework from earlier modules into a continuous-return Gaussian framework.

The objective is not to claim markets are perfectly Gaussian, but to:

- Generalize expectancy modeling
- Study aggregation effects
- Examine estimator instability
- Analyze drawdown behavior across horizons
- Verify volatility scaling assumptions

This module demonstrates how perception of risk changes under different evaluation frequencies — even when the underlying stochastic process remains unchanged.

---

## Submodules

### 6.1 — Aggregation

Using a stable IID Gaussian process:

- Daily returns were simulated
- Weekly and monthly returns were constructed via aggregation
- Volatility at each level was computed

Key Result:      
Volatility scales approximately with √time under IID assumptions.    

Insight:     
Smoother, higher-timeframe charts do not imply lower structural risk.    
Aggregation compresses visible noise but does not alter the underlying edge.       

---

### 6.2 — Rolling Window Instability

Using the same stationary process:

- Full-sample expectancy was computed
- Rolling expectancy windows of 20, 50, and 100 periods were compared

Key Result:     
Short evaluation windows exhibit large dispersion around the true mean.

Insight:     
Instability in rolling metrics does not imply regime change.      
It reflects estimator variance.       

Signal-to-noise ratio determines how quickly stability appears.

---

### 6.3 — Drawdown Across Horizons

Drawdowns were evaluated at:

- Trade-level resolution
- Weekly resolution
- Monthly resolution

Key Result:      
Maximum drawdown magnitude is structurally similar across horizons,     
but perceived severity changes.     

Insight:     
Risk perception is strongly dependent on sampling frequency.    
The same process can feel dramatically different depending on evaluation resolution.     

---

### 6.4 — Volatility Scaling & Misinterpretation

Volatility was computed at:

- Daily
- Weekly
- Monthly horizons

Square-root-of-time scaling was verified under IID assumptions.

A non-IID process with volatility clustering was then simulated.

Key Result:      
√time scaling holds under IID conditions but deviates when independence or constant variance assumptions are violated.      

Insight:   
Volatility scaling is conditional, not universal.    
Applying √time blindly can misestimate long-horizon risk.    

---

## Core Mathematical Principles

- Law of Large Numbers
- Standard Error of the Mean (σ / √n)
- Square-root-of-time volatility scaling
- Signal-to-noise ratio (μ / σ)
- Dependence on IID assumptions

---

## Key Takeaways

1. Aggregation changes perception, not expectancy.
2. Small samples exaggerate regime illusions.
3. Drawdown severity depends on evaluation frequency.
4. Volatility scaling requires independence and constant variance.
5. Timeframe does not create edge — signal-to-noise ratio determines stability.

---

## Practical Implications

- Rolling metrics must be interpreted relative to estimator variance.
- Short evaluation windows can falsely signal system breakdown.
- Higher timeframes may feel smoother but do not inherently reduce structural risk.
- Risk annualization using √time must be justified by structural assumptions.

---

## Conclusion

Module 6 formalizes how statistical structure interacts with perception.

The main lesson is not about which timeframe is superior.    
It is about understanding how variance, aggregation, and sampling affect the interpretation of performance and risk.    

Edge is structural.    
Perception is frequency-dependent.    
