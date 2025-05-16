# Timeout Strategy in the NFL: A Win Probability Analysis

## Overview

This project analyzes second-half timeout usage in NFL games, asking a strategic question often overlooked: _In the second half of games, when is it better to take a 5-yard penalty on offense rather than burn a timeout?_ Using historical play-by-play data, predictive modeling, and win probability simulations, the analysis identifies the conditions under which saving a timeout provides more long-term value than avoiding a minor loss of yardage.

The work was completed as a self-directed learning and analytics application project. All modeling, analysis, and code were developed independently, with guidance from available resources and large language models for coding support.

## Key Insights

- **Teams should take the penalty ~25% of the time** in second-half situations, especially in long-yardage, down-multiple-scores, or own-territory scenarios.
- **The first timeout is disproportionately valuable** — teams should be especially cautious about using it early.
- **Penalty cost varies sharply by field position and game context** — timeout strategy should adapt accordingly.

## Models Used

1. **Causal Modeling**: Estimated the marginal value of timeouts in late-game defensive stop scenarios.
2. **XGBoost Classifier**: Predicted the likelihood a team would need timeouts later to mount a comeback.
3. **Survival Model**: Estimated the time remaining until a team would face a potential late-game defensive drive, allowing for more accurate timeout value weighting.
4. **WP Replication**: Recreated nflfastR's win probability model to simulate the cost of delay-of-game penalties across thousands of second-half situations.

## Files

- `analysis_summary.pdf`: Full project write-up and key findings.
- `model_code.ipynb` / `.py`: Python code used for modeling, simulations, and visualizations.

## Why It Matters

Timeouts are among the most valuable — and underutilized — assets in football strategy. This project shows that with the right data and modeling, teams can gain a meaningful edge by optimizing how and when they use them.

## Project Link

📄 [Read the full analysis here (PDF)](./analysis_summary.pdf)  
🔗 [Live GitHub Repo](https://github.com/maeisen15/NFL_coding)
