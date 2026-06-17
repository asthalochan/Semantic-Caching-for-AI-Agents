# SemanticCacheOps Redis POC

This is a Redis-backed proof-of-concept notebook for a production-style semantic cache.

## Run

```bash
pip install -r requirements.txt
docker compose up -d
jupyter notebook SemanticCacheOps_Redis_POC.ipynb
```

## Optional OpenAI

```bash
export OPENAI_API_KEY="your_key_here"
```

Then enable the LLM validator cell by setting:

```python
RUN_LLM_VALIDATOR_DEMO = True
```

## What it demonstrates

- RedisVL SemanticCache
- Redis vector similarity search
- TTL
- Cache hit/miss flow
- OpenAI fallback on miss
- Threshold sweep
- Precision/recall/F1 evaluation
- Fuzzy matching
- Cross-encoder reranking
- Optional LLM validator
- Latency/cost-saving estimation
