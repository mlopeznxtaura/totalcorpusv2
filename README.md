# totalcorpusv2

Training corpus: 4 clusters x 20 SDKs x 20,000 runs x 10 cycles = **800,000 total runs**

## Clusters
- cluster_01: Language & Reasoning (20 SDKs)
- cluster_02: Vision & Multimodal (20 SDKs)  
- cluster_03: Audio & Speech (20 SDKs)
- cluster_04: Data & Embeddings (20 SDKs)

## Files
Each `.jsonl` file contains ~160,000 runs (~40MB). Files split across repos totalcorpusv2, totalcorpusv2.1, totalcorpusv2.2 etc when GitHub limit is hit.

## Schema
```json
{"run_id": "cluster_01_openai_1_00001", "cluster": "cluster_01", "sdk": "openai", "cycle": 1, "model": "gpt-4o", "task": "completion", "status": "success", "latency_s": 1.234, "tokens_in": 512, "tokens_out": 256, "cost_usd": 0.005376, "ts": "2026-05-01T00:01:00Z"}
```
