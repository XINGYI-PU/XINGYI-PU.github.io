---
layout: page
title: KIS Trading System and TinyGPT
description: An ECO4126 project combining safe trading-system simulation with a small decoder-only Transformer.
importance: 3
category: applied-ai
github: https://github.com/XINGYI-PU/ECO4126-Final-Project-KIS-TinyGPT
---

## Overview

This coursework repository contains two applied software projects: a simulation-first automated trading system designed around the Korea Investment & Securities Open API concept, and TinyGPT, a compact GPT-2-style language model implemented in PyTorch.

## KIS trading-system component

- Organizes the workflow as market data, strategy, risk management, order execution, and logging.
- Uses a moving-average crossover strategy to generate buy, sell, or hold signals.
- Applies position-size, daily-trade, stop-loss, and take-profit controls.
- Runs in simulation mode by default to prevent unintended real orders and credential exposure.

## TinyGPT component

- Implements token and positional embeddings, masked multi-head self-attention, feed-forward layers, residual connections, and layer normalization.
- Trains with character-level next-token prediction and cross-entropy loss.
- Supports checkpointing and autoregressive text generation.

**Technologies:** Python, PyTorch, Jupyter Notebook, Transformer architecture, API-oriented system design, and risk controls.

[View source code and documentation on GitHub](https://github.com/XINGYI-PU/ECO4126-Final-Project-KIS-TinyGPT).
