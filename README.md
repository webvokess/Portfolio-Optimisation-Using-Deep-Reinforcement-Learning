# Portfolio Optimization using Deep Reinforcement Learning

## Overview

This project explores a novel approach to portfolio optimization using deep reinforcement learning (DRL). By formulating portfolio optimization as a problem of sequential decision-making, we apply DRL methods to directly learn the optimal investment strategies from raw market data. Our study demonstrates the adaptability of DRL in adjusting to changing market conditions, surpassing state-of-the-art portfolio management tasks. We empirically evaluate our work on real-world financial data, showing our approach outperforms existing methods in terms of risk-adjusted returns and portfolio diversification performance.

## Introduction

Portfolio optimization aims to balance risk and return by constructing investment portfolios. Traditional methods like mean-variance optimization and Markowitz's portfolio theory have limitations in capturing market dynamics and nonlinear relationships among assets. Our project leverages DRL to overcome these challenges, employing algorithms such as Proximal Policy Optimization (PPO), Advantage Actor-Critic (A2C), and Soft Actor-Critic (SAC).

## DRL Framework

In our DRL framework, the key components are:

- **Agent**: A deep neural network that learns optimal portfolio allocations.
- **Actions**: The final weights assigned to each stock in the portfolio.
- **State**: The present market scenario, including asset values and prices.
- **Environment**: The trading market, providing rewards based on portfolio value changes.
- **Reward**: Reflects portfolio performance changes over time.

## Algorithms

We implemented and compared several DRL algorithms within our framework:

- **Actor-Critic (AC)**: Combines policy (actor) and value (critic) optimization.
- **Proximal Policy Optimization (PPO)**: Uses first-order optimization with bounded policy updates.
- **Advantage Actor-Critic (A2C)**: Reduces policy variance using advantage function estimates.
- **Soft Actor-Critic (SAC)**: Maximizes an objective including an entropy term for robust policy exploration.

## Experiments

Our experiments focused on asset allocation under different market conditions (bullish and bearish trends) using historical stock price data. We evaluated the performance of A2C, PPO, and SAC algorithms across various scenarios.

### Data

- **Bullish Market Trend**: Adjusted price data from 8 stocks (2010-2020).
- **Bearish Market Trend**: Adjusted price data from 9 stocks (2013-2024).

### Results

We conducted multiple runs to capture performance variability and compared DRL algorithms against traditional methods. Our findings indicate that DRL methods can outperform in specific market conditions, although performance consistency remains a challenge.

## Conclusion

Our study highlights the potential of DRL in portfolio optimization, demonstrating significant improvements in risk-adjusted returns and portfolio diversification. Future work could involve expanding the dataset, incorporating additional technical indicators, and refining DRL model architectures to enhance robustness and performance.

## References

A list of references cited in the project report.
