# Alpha Agent: Industrial-Grade Multi-Agent Based Framework for Alpha Research in Quantitative Investment
[![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-360/)
[![PyPI](https://img.shields.io/pypi/v/alphaagent.svg)](https://pypi.org/project/alphaagent/)
![License](https://img.shields.io/github/license/LLMQuant/alphaagent.svg?color=brightgreen)
![](https://img.shields.io/github/issues-raw/LLMQuant/alphaagent?label=Issues)
![](https://img.shields.io/github/issues-closed-raw/LLMQuant/alphaagent?label=Closed+Issues)
![](https://img.shields.io/github/issues-pr-raw/LLMQuant/alphaagent?label=Open+PRs)
![](https://img.shields.io/github/issues-pr-closed-raw/LLMQuant/alphaagent?label=Closed+PRs)

<div align="center">
<img align="center" width="40%" alt="image" src="https://github.com/LLMQuant/AlphaAgent/blob/main/AlphaAgent.png">
</div>

**AlphaAgent** is a practical and adaptive multi-agent framework for real-world quantitative research and development. Built upon the principles of [RD-Agent(Q)](https://arxiv.org/abs/2505.15155), it emphasizes **production-grade alpha discovery**, **market-aware modeling**, and **automated deployment**, leveraging live data streams, evolving knowledge bases, and robust backtesting infrastructure.

---

## 🌐 Core Objectives

AlphaAgent enables:
- Continuous mining and curation of high-value factor/model ideas from domain knowledge sources
- Dynamic retrieval of strategies that align with real-time market characteristics
- Self-refinement of hypotheses using prior experiments and contextual relevance
- Code generation, error correction, and backtest integration with minimal human intervention
- Automatic research documentation and decision support outputs for industrial use

## 🔁 System Pipeline

The full pipeline operates in a continuous feedback loop:

1. **Knowledge Base Construction**  
   Extract alpha factor and model ideas from large-scale research reports and academic papers via [`LLMQuant/quant-wiki`](https://github.com/LLMQuant/quant-wiki).

2. **Market Feature Extraction**  
   Continuously monitor financial news and macroeconomic updates via [`LLMQuant/MarketPulse`](https://github.com/LLMQuant/MarketPulse) to characterize market regimes (e.g., volatility, liquidity, sentiment, momentum).

3. **Contextual Retrieval & Hypothesis Generation**  
   Match current market regimes with relevant strategies from the internal knowledge base. Use similarity scoring and prior backtest records to refine retrieved hypotheses or generate novel ones.

4. **Code Synthesis**  
   Translate structured hypotheses into executable Python code using Co-STEER-style reasoning and knowledge transfer. Support chain-of-thought debugging and structured error recovery.

5. **Live Backtesting**  
   Deploy generated strategies into a Qlib-based real-time backtest pipeline. Evaluate under transaction cost, slippage, sector neutrality, and dynamic rebalancing conditions.

6. **Research Report Generation**  
   Summarize each experiment into human-readable research reports with metric tables, charts, diagnostics, and improvement suggestions.

> 🚧 AlphaAgent is under construction — exciting features and demos are coming soon. Stay tuned!

---

<p align="center"> <b>From Knowledge to Alpha</b><br> Made with ❤️ by <a href="https://github.com/LLMQuant">LLMQuant</a> </p>