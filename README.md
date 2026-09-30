# Pacman Ensemble Classifier Agent (Machine Learning)

> Three classifiers I wrote from scratch vote on Pacman's next move. One is a Bayesian network that learns its own structure.

🔒 The code sits in a private repository because this was King's College London coursework. Ask me and I'll walk you through it.

## Overview
The agent turns Pacman's surroundings (walls, food and nearby ghosts) into a binary feature vector and predicts a move. I trained it on a log of good moves and used no ML libraries.

## What I built
- **Nearest centroid classifier:** scores each direction by hand, rewarding food and safety and penalising walls and ghosts
- **k-nearest neighbours:** works on the raw vectors, with k = √N and random tie-breaks
- **Bayesian network:** a stochastic search picks the structure that maximises the Bayesian Information Criterion (BIC), then I estimate the probability tables and predict from the posterior
- **Voting:** a weighted vote combines the three models. If the winner picks an illegal move, the agent draws again

## Skills
Supervised learning · probabilistic graphical models · feature engineering · ensembles

## Tech stack
Python, with no ML libraries
