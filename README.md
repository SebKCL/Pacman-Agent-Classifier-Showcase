# Pacman Ensemble Classifier Agent (Machine Learning)

> A Pacman controller driven by an ensemble of three classifiers written from scratch, including a Bayesian network that learns its own structure.

🔒 **The source code is in a private repository** because this was university coursework at King's College London. I'm happy to walk through the code on request.

## Overview
The agent turns Pacman's local surroundings (walls, food and nearby ghosts) into a binary feature vector and predicts the best move. It was trained on a dataset of logged "good moves". All the models are my own implementations, with no ML libraries.

## What I built
- **Nearest Centroid Classifier:** built on hand-engineered directional scores that reward food and safety and penalise walls and ghosts
- **k-Nearest Neighbours:** works on the raw feature vectors, with k = √N and random tie-breaking
- **Bayesian network:** structure learned by a stochastic search that maximises the Bayesian Information Criterion (BIC), with conditional probability table (CPT) estimation and posterior-based prediction
- **Weighted-voting ensemble:** combines the three models' predictions and enforces move legality, re-sampling whenever the chosen move is illegal

## Skills demonstrated
Supervised learning · probabilistic graphical models · feature engineering · ensemble methods · implementing algorithms from scratch

## Tech stack
Python (no external ML libraries)
