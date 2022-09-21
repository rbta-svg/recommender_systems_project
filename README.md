# Recommender System 2021 Challenge (Politecnico di Milano)
## Goal

The application domain is TV programs recommendation. The datasets we provide contains both interactions between users and TV shows, as well as features related to the shows. The main goal of the competition is to discover which items (TV shows) a user will interact with.
Each TV show (for instance, "The Big Bang Theory") can be composed by several episodes (for instance, episode 5, season 3). The goal of the recommender system is not recommend a specific episode, but to recommend the TV show.

## Description

The datasets includes around 6.2M interactions, 13k users, 18k items (TV shows) and four feature categories: 8 genres, 213 channels, 113 subgenres and 358k events (episode ids).
The training-test split is done via random holdout, 85% training, 15% test.
The goal is to recommend a list of 10 potentially relevant items for each user. MAP@10 is used for evaluation. Any kind of python-written recommender system was allowed.

## Solution
Several techniques have been tested, such as RP3 Beta, Matrix Factorization, SLIM, also merged through various methods to create hybrid models. Hyperparameter optimization techniques were also used to find the optimal parameters.

The best submission score was obtained using a SLIM ElasticNet, with the hyperparameters being optimized through a Bayesian search.

Final outcome are as follows:
- Baselines: 12/12 passed
- Public Leaderboard: 34/85 (MAP@10: 0.47699 - highest in the competition: 0.51098)
- Private Leaderboard: 34/85 (MAP@10: 0.47727 - highest in the competition:0.50966)

Please note that many of the implemented techniques were forked and modified from the competition [repository](https://github.com/MaurizioFD/RecSys_Course_AT_PoliMi).

## Looking forward
Further experiment with neural recommenders is to be done, for learning sake (the competition is already over). Please come back later! 




