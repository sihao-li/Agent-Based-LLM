# Enriching Agent-Based Modeling with LLM-Driven MBTI Personalities

This repository contains the source code and associated report for the research project titled “Enriching Agent-Based Modeling’s with LLM-driven MBTI Personalities: A Benchmark Framework.” The project implements a macroeconomic sandbox where heterogeneous agents, each assigned an MBTI personality profile, make economic decisions via a Large Language Model (LLM).

🚀 Key Features

Based on Park & al. 2023 and https://github.com/mkturkcan/generative-agents
- Simulates a closed economy (consumption, investment, borrowing) inspired by a stylized village (Phandalin).
- Uses Llama‑3.2‑7B‑Instruct as the decision engine, generating textual narratives that are parsed into economic actions.
- Assigns each agent one of the 16 MBTI types, influencing decision-making (distribution aligned with empirical proportions).
- Agents store a history of interactions (transactions, social events) to inform future decisions.
- Converts raw logs into structured tuples (action, object, amount, MBTI, wealth) and aggregates macro indicators (consumption, investment, borrowing, average wealth).

## Install

```bash
git clone https://github.com/sihao-li/Agent-Based-LLM/
cd your-repo
```

If you're using Llama-3.2-7B-Instruct, don't forget to retrieve your token from Huggingface :
```bash
!pip install huggingface_hub
from huggingface_hub import login
access_token_write = "YOUR_HUGGINGFACE_TOKEN"  # Replace with your Hugging Face token
login(token = access_token_write)
```

## Citation

Li, S. H., & Carnapete, O. (2024). Enriching agent-based modeling’s with LLM-driven MBTI personalities: A benchmark framework. Université Paris Dauphine.


