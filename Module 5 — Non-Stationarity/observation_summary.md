# Module 5 — Non-Stationarity & Edge Instability
## Core Focus
This module studies how win rate and edge behave under changing regimes, even when long-term expectancy appears stable.    

The central question:     
> How reliable is edge evaluation when the underlying process is not stationary?

--- 
## 5.1 — Drifting Expectancy
Even with constant win probability, outcomes cluster.

### Observation:

- Short-term win rate fluctuates heavily.
- Streaks create the illusion of regime change.
- Small samples exaggerate perceived edge strength or decay.

### Takeaway:
- Observed win rate is unstable in small samples, even when the true edge is constant.
- True edge is never directly observable — only estimated with uncertainty.
  
---
## 5.2 — Abrupt Regime Switch
Edge detection is inherently delayed due to rolling window smoothing.

### Observation:

- A simple rolling threshold (<50%) produces a very high false alarm rate when the true edge is only moderately above 50%.
- Even a clear structural break (55% → 44%) is difficult to detect cleanly in real time.

### Takeaway:   
- True edge is unobservable.
- Regime detection is probabilistic, not certain.

--- 
### 5.3 — Volatility Regime Shift
Variance increases while win rate and expectancy remain constant.

### Observation:

- Higher variance produces deeper drawdowns.
- Recovery periods become longer.
- Emotional stress increases despite an unchanged edge.

### Takeaway:
Edge can remain constant while perceived performance deteriorates.

--- 
## 5.4 — Random Structural Break Timing
Win rate shifts randomly and may revert later.

### Observation:

- Rolling win rate lags true regime changes.
- Breaks are statistically ambiguous in real time.
- Hindsight makes regime shifts appear obvious.

### Takeaway:
Edge decay and variance are difficult to distinguish in real time.     
Detection requires large samples, creating an unavoidable delay.   

---
## Final Conclusion
Win rate is not a stable observable in small or medium samples.

Under non-stationarity:

- True edge may temporarily disappear.
- Observed performance may mislead.
- Detection of structural change is delayed and probabilistic.
- Evaluation depends heavily on the sample window and path.

Edge exists as a long-run property.      
What traders observe is a noisy, path-dependent estimate.    

Misinterpreting that estimate leads to:

- Premature abandonment of valid systems
- Holding broken systems too long
- Emotional overreaction to normal variance

The central lesson:    

**Non-stationarity makes edge evaluation inherently unstable.**








