# Contributing to Adaptive RecSys

## Setup
```bash
git clone https://github.com/yourusername/adaptive-recsys.git
cd adaptive-recsys
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt && pip install -e .
```

## Priority Areas
1. **New RL algorithms** (SAC, TD3, RAINBOW DQN)
2. **GNN models** (completing LightGCN, NGCF training loops)
3. **Real Kafka streaming** integration
4. **Federated Learning** for privacy-preserving recs
5. **Causal RL** for recommendation (debiasing)
6. **LLM integration** (prompting for explanation generation)
7. **Evaluation benchmarks** (full MovieLens-25M training)

## Tests
```bash
python tests/test_all.py     # Quick (no pytest needed)
pytest tests/ -v --cov=src   # With coverage
```

## Commit Convention
```
feat: add SAC agent for continuous action spaces
fix: ADWIN window size underflow at initialization
research: add LightGCN convergence analysis notebook
data: add RetailRocket dataset downloader script
```

## Research Contributions
If you're adding a new algorithm, please include:
- Paper reference (authors, year, venue, arXiv ID)
- Pseudocode in the docstring
- Unit test with expected behavior
- Benchmark comparison in the notebook
