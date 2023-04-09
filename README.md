# Wordle Bot

This is a Wordle bot that uses a probabilistic approach based on concepts from entropy and information theory to find the best pick for the first guess. Based on the findings with the limited dataset, it usually takes 2.6 steps on average to find the right word. 

This wordle bot tries to make guesses that reduce the entropy as much as possible. We will do this by calculating the expected information gain for each possible word in our dataset and subsequently pick the best candidate word.

The definition of entropy $H(X)$ for a discrete random variable $X$ is the expected amount of information content: $\mathbb{E}[I(X)]$. Here, the information content $I(X)$ is defined as : $I(X) = \log_2\left(\frac{1}{p(X)}\right)$.

Assumption: each word in the dataset to be equaly likely to be the daily word.