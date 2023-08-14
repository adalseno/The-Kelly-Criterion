This is a fork of [The Kelly Criterion](https://github.com/1kc2/The-Kelly-Criterion) by [ikc2](https://github.com/1kc2and) and uses `numba` in `utils.py` to speed up the computation for correlated assets ($\approx 53X$ faster on the same dataset). 
My setup:

- numpy 1.23.5
- numba 0.57.1
- pandas 2.0.3
- python 3.9.15
- matplotlib 3.7.2
- seaborn 0.12.2

You must have `numba` installed and should match the same setup to avoid issues. Different versions may work but haven't been tested.

Run in [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/adalseno/The-Kelly-Criterion/HEAD?labpath=The%20Kelly%20Criterion.ipynb)

# The Kelly Criterion

> This is the accompanying Jupyter Notebook for this [blog](https://blog.karanc.me/2020/10/21/the-kelly-criterion-part-2) post.

When investing, we spend plenty of time thinking about which securities should we buy but we rarely wonder how much money should we allocate in each asset.

Although it does not seem like an important aspect, it is crucial when defining a strategy, up to the point that it can determine the whole performance of your portfolio.

In this sense, the Kelly criterion helps us selecting the optimal proportion such that we can maximize our expected returns.

There have been many papers and books written about the Kelly criteria and its characteristics. In this notebook we will see an introduction for the Kelly criterion in continuous time and it's uses for the stock market. This notebook's aim is to serve as a starting point to understand and apply the Kelly criterion in the stock market. Personally, I find the Kelly Criterion fascinating for it's simplicity, elegance and utility.
