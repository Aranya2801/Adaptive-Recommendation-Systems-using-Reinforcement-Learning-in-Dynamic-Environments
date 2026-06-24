# Changelog

## [2.0.0] — 2026-06-14

### Added — Research Modules
- 5 Bandit algorithms: ε-Greedy, UCB1, Thompson Sampling, LinUCB, NeuralUCB
- 5 RL Agents: DQN, Double DQN, Dueling DQN, PPO, A2C
- Prioritized Experience Replay (PER) with importance sampling
- 3 Sequential models: GRU4Rec, SASRec, BERT4Rec
- Classical models: MF (ALS-SGD), FunkSVD, NCF
- Adaptive Fusion Layer: Weighted, Contextual, Meta-Bandit strategies
- Drift Detection: ADWIN, Page-Hinkley, KS-WIN, Preference Drift Tracker
- Daily Adaptive Intelligence Engine (10 domains, behavioral learning)
- FastAPI server with 18 endpoints + WebSocket streaming

### Performance
- 115/115 unit tests passing
- Benchmark: Adaptive Fusion achieves HR@10=0.513, NDCG@10=0.371 on simulated data
- All inference < 100ms (bandit/RL < 10ms, sequential 30-50ms)

### Research References
- Mnih et al. (2015) DQN — Nature
- Schulman et al. (2017) PPO — arXiv
- Li et al. (2010) LinUCB — WWW
- Sun et al. (2019) BERT4Rec — CIKM
- Kang & McAuley (2018) SASRec — ICDM
- Bifet & Gavalda (2007) ADWIN — SDM
