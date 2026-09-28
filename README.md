# Bayesian Modeling of Athletic Performance

A complete Bayesian inference pipeline in Python that models an athlete's performance scores over time, moving from a simple conjugate update to a custom MCMC sampler for a latent-variable mixture model.

The notebook has all outputs and plots saved, so you can read the full analysis directly on GitHub without running anything.

## Pipeline

1. **Prior estimation**: estimated a prior distribution for performance scores from several years of historical data
2. **Conjugate Bayesian update**: applied a normal-normal conjugate update to compute the posterior distribution after observing a new season's data
3. **Latent-variable mixture model**: extended the model to separate two latent performance regimes ("prepared" vs. "unprepared"), since a single normal distribution did not adequately capture the observed variance
4. **Custom Gibbs sampler (MCMC)**: implemented a Gibbs sampler from scratch to infer the mixture model's parameters
5. **Posterior predictive distribution**: generated predictive distributions for future performance based on the fitted model

## Tech Stack

Python, NumPy, SciPy, statsmodels, Matplotlib, Seaborn

## How to Run

```bash
pip install numpy scipy statsmodels matplotlib seaborn jupyter
jupyter notebook bayesian_athletic_performance.ipynb
```

## Author

Maryam Taghinasab, individual project, Statistical Methods course, University of Tehran
