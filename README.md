# Fb Betting Graph

_(credit to @notadamking, [this repo](https://github.com/notadamking/Stock-Trading-Visualization) and [this article](https://towardsdatascience.com/visualizing-stock-trading-agents-using-matplotlib-and-gym-584c992bc6d4))_

This repository contains a Jupyter Notebook (`source/OHCL FB Bet Graph.ipynb`) with a custom class `FootballBettingGraph` that visualises bets (balance, profit, volumes, individual bets).

The idea is similar to what Stock Traders would use to visualise market movements, applied to Football Betting. This can be used to visualise the training process of a model and how it makes decisions when to bet. The class can also be adopted to plot bets real-time.

Includes some test data (`source/test_data.xlsx`) and an example on how to run the graph using that data.

## Installing
Clone the repo, install dependencies, open `OHCL FB Bet Graph.ipynb` using Jupyter Notebook (or something else) and run it.

## Requirements

See `requirements.txt`.

## Improvements
- `_render_balance` can use `plot_date` to create a more dynamic visualisation of bets. However, this would tie the implementation down to using dates
- `Profit` column is redundant as it can be calculated from the opening and closing values
- in volumes, display more details about the type of bets (win? lose? something else?)