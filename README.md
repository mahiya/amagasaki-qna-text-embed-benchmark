# テキスト埋め込みモデル 日本語性能ベンチマーク

## データセット: 尼崎市 Q&A データセット

京都大学が公開している BERT-Based FAQ Retrieval 用データセットを使用しています。

- [BERT-Based FAQ Retrieval (京都大学)](https://nlp.ist.i.kyoto-u.ac.jp/EN/index.php?BERT-Based_FAQ_Retrieval)
- [GitHub リポジトリ](https://github.com/ku-nlp/bert-based-faqir)

| 項目 | 内容 |
|------|------|
| コーパス | 尼崎市の Q&A ドキュメント 1,785 件 |
| クエリ | 検索クエリ 748 件 |
| 適合性判定 (qrels) | クエリとドキュメントのペアに対する関連度スコア (1: やや関連, 2: 高関連) |

## ベンチマークの結果

### Recall@10

| Rank | Publisher | Model | Parameter Size | Release Date | Score |
|------|-----------|-------|---------------|-------------|-------|
| 1 | NVIDIA | [nemotron-3.5-rerank-8b](https://huggingface.co/nvidia/Nemotron-3.5-Rerank-8B-BF16) | 8.4B | 2026-10 | 0.895 |
| 2 | Perplexity | [pplx-embed-v2-late-9b](https://huggingface.co/perplexity-ai/pplx-embed-v2-late-9b) | 8.4B | 2026-10 | 0.866 |
| 3 | Cohere | [cohere-rerank-v5.0-pro](https://docs.cohere.com/docs/rerank) |  | 2026-10 | 0.865 |
| 4 | Perplexity | [pplx-embed-v2-late-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v2-late-0.6b) | 0.6B | 2026-10 | 0.860 |
| 5 | SB Intuitions | [sarashina3-rerank](https://docs.sarashina.ai/api-reference/rerank) |  | 2026-07 | 0.852 |
| 6 | Cohere | [cohere-rerank-v5.0-fast](https://docs.cohere.com/docs/rerank) |  | 2026-10 | 0.837 |
| 7 | Cohere | [cohere-embed-v5.0-pro](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.832 |
| 8 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.823 |
| 9 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.821 |
| 10 | SB Intuitions | [sarashina3-embedding](https://docs.sarashina.ai/api-reference/embeddings) |  | 2026-07 | 0.817 |
| 11 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.814 |
| 12 | Perplexity | [pplx-embed-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-v1-4b) | 4B | 2026-02 | 0.814 |
| 13 | Perplexity | [pplx-embed-v2-context-9b-preview](https://huggingface.co/perplexity-ai/pplx-embed-v2-context-9b-preview) | 8.4B | 2026-09 | 0.808 |
| 14 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.806 |
| 15 | Nagoya University | [ruri-v3-reranker-310m](https://huggingface.co/cl-nagoya/ruri-v3-reranker-310m) | 0.31B | 2025-04 | 0.805 |
| 16 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.802 |
| 17 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.802 |
| 18 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.801 |
| 19 | Cohere | [cohere-embed-v5.0-fast](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.797 |
| 20 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.792 |
| 21 | Perplexity | [pplx-embed-context-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-4b) | 4B | 2026-02 | 0.786 |
| 22 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.786 |
| 23 | NVIDIA | [nemotron-3-embed-1b-nvfp4](https://huggingface.co/nvidia/Nemotron-3-Embed-1B-NVFP4) | 1.14B | 2026-07 | 0.784 |
| 24 | NVIDIA | [nemotron-3.5-embed-8b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-8B-BF16) | 8.4B | 2026-10 | 0.783 |
| 25 | NVIDIA | [nemotron-3-embed-8b](https://huggingface.co/nvidia/Nemotron-3-Embed-8B-BF16) | 7.95B | 2026-07 | 0.783 |
| 26 | NVIDIA | [nemotron-3.5-embed-1b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-1B-BF16) | 1.55B | 2026-10 | 0.782 |
| 27 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.780 |
| 28 | NVIDIA | [nemotron-3-embed-1b](https://huggingface.co/nvidia/Nemotron-3-Embed-1B-BF16) | 1.14B | 2026-07 | 0.780 |
| 29 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.778 |
| 30 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.773 |
| 31 | Sionic AI | [comsat-embed-ja-8b-preview](https://huggingface.co/sionic-ai/comsat-embed-ja-8b-preview) | 7.57B | 2026-07 | 0.771 |
| 32 | Perplexity | [pplx-embed-context-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-0.6b) | 0.6B | 2026-02 | 0.769 |
| 33 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.765 |
| 34 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.762 |
| 35 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.761 |
| 36 | Alibaba | [qwen3-reranker-0.6b](https://huggingface.co/Qwen/Qwen3-Reranker-0.6B) | 0.6B | 2025-06 | 0.761 |
| 37 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.756 |
| 38 | Jina AI | [jina-embeddings-v5-omni-small](https://huggingface.co/jinaai/jina-embeddings-v5-omni-small) | 1.74B | 2026-05 | 0.755 |
| 39 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.753 |
| 40 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.751 |
| 41 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.745 |
| 42 | Sionic AI | [comsat-embed-ja-0.3b-preview](https://huggingface.co/sionic-ai/comsat-embed-ja-0.3b-preview) | 0.31B | 2026-07 | 0.742 |
| 43 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.740 |
| 44 | Jina AI | [jina-embeddings-v5-omni-nano](https://huggingface.co/jinaai/jina-embeddings-v5-omni-nano) | 1.04B | 2026-05 | 0.740 |
| 45 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.738 |
| 46 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.735 |
| 47 | Google | [embeddinggemma-2](https://huggingface.co/google/embeddinggemma-2) | 0.74B | 2026-10 | 0.735 |
| 48 | Jina AI | [jina-reranker-v3.5](https://huggingface.co/jinaai/jina-reranker-v3.5) | 0.6B | 2026-07 | 0.733 |
| 49 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.723 |
| 50 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.719 |
| 51 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.715 |
| 52 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.710 |
| 53 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.706 |
| 54 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.701 |
| 55 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.698 |
| 56 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.683 |
| 57 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.682 |
| 58 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.664 |
| 59 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.660 |
| 60 | Jina AI | [jina-reranker-v3](https://huggingface.co/jinaai/jina-reranker-v3) | 0.6B | 2025-09 | 0.646 |
| 61 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.645 |
| 62 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.642 |
| 63 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.615 |
| 64 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.600 |
| 65 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.566 |
| 66 | Jina AI | [jina-colbert-v2-64](https://huggingface.co/jinaai/jina-colbert-v2-64) | 0.56B | 2024-08 | 0.560 |
| 67 | Jina AI | [jina-colbert-v2](https://huggingface.co/jinaai/jina-colbert-v2) | 0.56B | 2024-08 | 0.557 |
| 68 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.528 |
| 69 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.511 |
| 70 | Yuichi Tateno | [bekko-static-embedding-v1](https://huggingface.co/hotchpotch/bekko-static-embedding-v1) | 0.2B | 2026-09 | 0.482 |
| 71 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.462 |
| 72 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.247 |
| 73 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.199 |
| 74 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.180 |
| 75 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.133 |
| 76 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.130 |

### Precision@10

| Rank | Publisher | Model | Parameter Size | Release Date | Score |
|------|-----------|-------|---------------|-------------|-------|
| 1 | NVIDIA | [nemotron-3.5-rerank-8b](https://huggingface.co/nvidia/Nemotron-3.5-Rerank-8B-BF16) | 8.4B | 2026-10 | 0.204 |
| 2 | Perplexity | [pplx-embed-v2-late-9b](https://huggingface.co/perplexity-ai/pplx-embed-v2-late-9b) | 8.4B | 2026-10 | 0.197 |
| 3 | Cohere | [cohere-rerank-v5.0-pro](https://docs.cohere.com/docs/rerank) |  | 2026-10 | 0.197 |
| 4 | Perplexity | [pplx-embed-v2-late-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v2-late-0.6b) | 0.6B | 2026-10 | 0.196 |
| 5 | SB Intuitions | [sarashina3-rerank](https://docs.sarashina.ai/api-reference/rerank) |  | 2026-07 | 0.194 |
| 6 | Cohere | [cohere-rerank-v5.0-fast](https://docs.cohere.com/docs/rerank) |  | 2026-10 | 0.192 |
| 7 | Cohere | [cohere-embed-v5.0-pro](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.191 |
| 8 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.188 |
| 9 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.187 |
| 10 | SB Intuitions | [sarashina3-embedding](https://docs.sarashina.ai/api-reference/embeddings) |  | 2026-07 | 0.187 |
| 11 | Perplexity | [pplx-embed-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-v1-4b) | 4B | 2026-02 | 0.186 |
| 12 | Nagoya University | [ruri-v3-reranker-310m](https://huggingface.co/cl-nagoya/ruri-v3-reranker-310m) | 0.31B | 2025-04 | 0.186 |
| 13 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.185 |
| 14 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.185 |
| 15 | Cohere | [cohere-embed-v5.0-fast](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.184 |
| 16 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.184 |
| 17 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.183 |
| 18 | Perplexity | [pplx-embed-v2-context-9b-preview](https://huggingface.co/perplexity-ai/pplx-embed-v2-context-9b-preview) | 8.4B | 2026-09 | 0.183 |
| 19 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.182 |
| 20 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.181 |
| 21 | NVIDIA | [nemotron-3.5-embed-8b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-8B-BF16) | 8.4B | 2026-10 | 0.181 |
| 22 | NVIDIA | [nemotron-3-embed-8b](https://huggingface.co/nvidia/Nemotron-3-Embed-8B-BF16) | 7.95B | 2026-07 | 0.180 |
| 23 | NVIDIA | [nemotron-3.5-embed-1b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-1B-BF16) | 1.55B | 2026-10 | 0.180 |
| 24 | NVIDIA | [nemotron-3-embed-1b-nvfp4](https://huggingface.co/nvidia/Nemotron-3-Embed-1B-NVFP4) | 1.14B | 2026-07 | 0.180 |
| 25 | NVIDIA | [nemotron-3-embed-1b](https://huggingface.co/nvidia/Nemotron-3-Embed-1B-BF16) | 1.14B | 2026-07 | 0.179 |
| 26 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.178 |
| 27 | Perplexity | [pplx-embed-context-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-4b) | 4B | 2026-02 | 0.178 |
| 28 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.177 |
| 29 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.177 |
| 30 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.177 |
| 31 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.177 |
| 32 | Perplexity | [pplx-embed-context-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-0.6b) | 0.6B | 2026-02 | 0.175 |
| 33 | Sionic AI | [comsat-embed-ja-8b-preview](https://huggingface.co/sionic-ai/comsat-embed-ja-8b-preview) | 7.57B | 2026-07 | 0.175 |
| 34 | Jina AI | [jina-embeddings-v5-omni-small](https://huggingface.co/jinaai/jina-embeddings-v5-omni-small) | 1.74B | 2026-05 | 0.174 |
| 35 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.174 |
| 36 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.174 |
| 37 | Jina AI | [jina-embeddings-v5-omni-nano](https://huggingface.co/jinaai/jina-embeddings-v5-omni-nano) | 1.04B | 2026-05 | 0.174 |
| 38 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.174 |
| 39 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.173 |
| 40 | Alibaba | [qwen3-reranker-0.6b](https://huggingface.co/Qwen/Qwen3-Reranker-0.6B) | 0.6B | 2025-06 | 0.173 |
| 41 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.172 |
| 42 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.172 |
| 43 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.172 |
| 44 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.171 |
| 45 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.171 |
| 46 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.170 |
| 47 | Google | [embeddinggemma-2](https://huggingface.co/google/embeddinggemma-2) | 0.74B | 2026-10 | 0.169 |
| 48 | Sionic AI | [comsat-embed-ja-0.3b-preview](https://huggingface.co/sionic-ai/comsat-embed-ja-0.3b-preview) | 0.31B | 2026-07 | 0.168 |
| 49 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.167 |
| 50 | Jina AI | [jina-reranker-v3.5](https://huggingface.co/jinaai/jina-reranker-v3.5) | 0.6B | 2026-07 | 0.166 |
| 51 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.163 |
| 52 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.163 |
| 53 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.163 |
| 54 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.159 |
| 55 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.159 |
| 56 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.158 |
| 57 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.158 |
| 58 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.153 |
| 59 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.151 |
| 60 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.148 |
| 61 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.148 |
| 62 | Jina AI | [jina-reranker-v3](https://huggingface.co/jinaai/jina-reranker-v3) | 0.6B | 2025-09 | 0.144 |
| 63 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.142 |
| 64 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.137 |
| 65 | Jina AI | [jina-colbert-v2-64](https://huggingface.co/jinaai/jina-colbert-v2-64) | 0.56B | 2024-08 | 0.132 |
| 66 | Jina AI | [jina-colbert-v2](https://huggingface.co/jinaai/jina-colbert-v2) | 0.56B | 2024-08 | 0.131 |
| 67 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.123 |
| 68 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.121 |
| 69 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.119 |
| 70 | Yuichi Tateno | [bekko-static-embedding-v1](https://huggingface.co/hotchpotch/bekko-static-embedding-v1) | 0.2B | 2026-09 | 0.109 |
| 71 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.108 |
| 72 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.056 |
| 73 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.042 |
| 74 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.038 |
| 75 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.032 |
| 76 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.021 |

### nDCG@10

| Rank | Publisher | Model | Parameter Size | Release Date | Score |
|------|-----------|-------|---------------|-------------|-------|
| 1 | NVIDIA | [nemotron-3.5-rerank-8b](https://huggingface.co/nvidia/Nemotron-3.5-Rerank-8B-BF16) | 8.4B | 2026-10 | 0.811 |
| 2 | Perplexity | [pplx-embed-v2-late-9b](https://huggingface.co/perplexity-ai/pplx-embed-v2-late-9b) | 8.4B | 2026-10 | 0.751 |
| 3 | Cohere | [cohere-rerank-v5.0-pro](https://docs.cohere.com/docs/rerank) |  | 2026-10 | 0.744 |
| 4 | Perplexity | [pplx-embed-v2-late-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v2-late-0.6b) | 0.6B | 2026-10 | 0.738 |
| 5 | SB Intuitions | [sarashina3-rerank](https://docs.sarashina.ai/api-reference/rerank) |  | 2026-07 | 0.736 |
| 6 | SB Intuitions | [sarashina3-embedding](https://docs.sarashina.ai/api-reference/embeddings) |  | 2026-07 | 0.727 |
| 7 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.725 |
| 8 | Cohere | [cohere-rerank-v5.0-fast](https://docs.cohere.com/docs/rerank) |  | 2026-10 | 0.722 |
| 9 | Nagoya University | [ruri-v3-reranker-310m](https://huggingface.co/cl-nagoya/ruri-v3-reranker-310m) | 0.31B | 2025-04 | 0.715 |
| 10 | Perplexity | [pplx-embed-v2-context-9b-preview](https://huggingface.co/perplexity-ai/pplx-embed-v2-context-9b-preview) | 8.4B | 2026-09 | 0.711 |
| 11 | Perplexity | [pplx-embed-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-v1-4b) | 4B | 2026-02 | 0.710 |
| 12 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.708 |
| 13 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.707 |
| 14 | Cohere | [cohere-embed-v5.0-pro](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.704 |
| 15 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.696 |
| 16 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.691 |
| 17 | Perplexity | [pplx-embed-context-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-4b) | 4B | 2026-02 | 0.689 |
| 18 | Cohere | [cohere-embed-v5.0-fast](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.686 |
| 19 | NVIDIA | [nemotron-3-embed-8b](https://huggingface.co/nvidia/Nemotron-3-Embed-8B-BF16) | 7.95B | 2026-07 | 0.685 |
| 20 | NVIDIA | [nemotron-3.5-embed-8b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-8B-BF16) | 8.4B | 2026-10 | 0.685 |
| 21 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.681 |
| 22 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.666 |
| 23 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.666 |
| 24 | NVIDIA | [nemotron-3.5-embed-1b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-1B-BF16) | 1.55B | 2026-10 | 0.664 |
| 25 | NVIDIA | [nemotron-3-embed-1b](https://huggingface.co/nvidia/Nemotron-3-Embed-1B-BF16) | 1.14B | 2026-07 | 0.664 |
| 26 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.663 |
| 27 | NVIDIA | [nemotron-3-embed-1b-nvfp4](https://huggingface.co/nvidia/Nemotron-3-Embed-1B-NVFP4) | 1.14B | 2026-07 | 0.663 |
| 28 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.662 |
| 29 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.659 |
| 30 | Perplexity | [pplx-embed-context-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-0.6b) | 0.6B | 2026-02 | 0.655 |
| 31 | Sionic AI | [comsat-embed-ja-8b-preview](https://huggingface.co/sionic-ai/comsat-embed-ja-8b-preview) | 7.57B | 2026-07 | 0.653 |
| 32 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.652 |
| 33 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.649 |
| 34 | Jina AI | [jina-reranker-v3.5](https://huggingface.co/jinaai/jina-reranker-v3.5) | 0.6B | 2026-07 | 0.648 |
| 35 | Sionic AI | [comsat-embed-ja-0.3b-preview](https://huggingface.co/sionic-ai/comsat-embed-ja-0.3b-preview) | 0.31B | 2026-07 | 0.644 |
| 36 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.642 |
| 37 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.637 |
| 38 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.637 |
| 39 | Alibaba | [qwen3-reranker-0.6b](https://huggingface.co/Qwen/Qwen3-Reranker-0.6B) | 0.6B | 2025-06 | 0.634 |
| 40 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.634 |
| 41 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.633 |
| 42 | Jina AI | [jina-embeddings-v5-omni-small](https://huggingface.co/jinaai/jina-embeddings-v5-omni-small) | 1.74B | 2026-05 | 0.628 |
| 43 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.628 |
| 44 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.625 |
| 45 | Jina AI | [jina-embeddings-v5-omni-nano](https://huggingface.co/jinaai/jina-embeddings-v5-omni-nano) | 1.04B | 2026-05 | 0.625 |
| 46 | Google | [embeddinggemma-2](https://huggingface.co/google/embeddinggemma-2) | 0.74B | 2026-10 | 0.625 |
| 47 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.620 |
| 48 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.612 |
| 49 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.600 |
| 50 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.597 |
| 51 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.590 |
| 52 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.590 |
| 53 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.589 |
| 54 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.587 |
| 55 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.586 |
| 56 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.586 |
| 57 | Jina AI | [jina-reranker-v3](https://huggingface.co/jinaai/jina-reranker-v3) | 0.6B | 2025-09 | 0.576 |
| 58 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.571 |
| 59 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.556 |
| 60 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.555 |
| 61 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.522 |
| 62 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.521 |
| 63 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.495 |
| 64 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.494 |
| 65 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.486 |
| 66 | Jina AI | [jina-colbert-v2-64](https://huggingface.co/jinaai/jina-colbert-v2-64) | 0.56B | 2024-08 | 0.465 |
| 67 | Jina AI | [jina-colbert-v2](https://huggingface.co/jinaai/jina-colbert-v2) | 0.56B | 2024-08 | 0.465 |
| 68 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.411 |
| 69 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.407 |
| 70 | Yuichi Tateno | [bekko-static-embedding-v1](https://huggingface.co/hotchpotch/bekko-static-embedding-v1) | 0.2B | 2026-09 | 0.395 |
| 71 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.356 |
| 72 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.188 |
| 73 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.170 |
| 74 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.127 |
| 75 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.111 |
| 76 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.088 |

## 評価方法

### 埋め込みの生成

各モデルを使用して、コーパス (ドキュメント) とクエリのテキストをベクトルに変換します。モデルによっては、クエリとドキュメントで異なるプレフィックスや `input_type` パラメータを指定しています。

### 検索 (Retrieval)

Elasticsearch の kNN (k-Nearest Neighbors) 検索を使用しています。

| 項目 | 設定値 |
|------|--------|
| 類似度関数 | コサイン類似度 |
| インデックスアルゴリズム | HNSW (Hierarchical Navigable Small World) |
| HNSW パラメータ | m=32, ef_construction=128 |
| 検索候補数 | 1,000 (num_candidates) |
| 取得件数 | 上位 100 件 |

各クエリのベクトルに対して、コーパス内のベクトルとのコサイン類似度が高い上位 100 件のドキュメントを取得し、その結果を評価メトリクスで評価します。

### 評価メトリクス

すべてのメトリクスは **k=10** で評価しています。Elasticsearch の [Ranking Evaluation API](https://www.elastic.co/docs/reference/elasticsearch/rest-apis/search-rank-eval) を使用して算出しています。

#### Recall@10
上位 10 件に含まれる関連ドキュメントの割合 (網羅性)。

$$\text{Recall@10} = \frac{\text{上位10件中の関連ドキュメント数}}{\text{全関連ドキュメント数}}$$

#### Precision@10
上位 10 件のうち関連ドキュメントである割合 (精度)。

$$\text{Precision@10} = \frac{\text{上位10件中の関連ドキュメント数}}{10}$$

#### nDCG@10 (Normalized Discounted Cumulative Gain)
ランキングの順位と関連度を考慮した評価指標。上位に高関連のドキュメントが来るほど高スコアとなります。

$$\text{DCG@10} = \sum_{i=1}^{10} \frac{rel_i}{\log_2(i+1)}$$

$$\text{nDCG@10} = \frac{\text{DCG@10}}{\text{Ideal DCG@10}}$$

### リランキング (Reranking)

第 1 段階の埋め込みモデルで上位 100 文書を取得し、第 2 段階のリランカーで同じ 100 文書を並べ替える 2 段階検索を測定しています。リランカーは候補の順序だけを変えるため、第 1 段階が上位 100 件に入れられなかった関連文書は回収できません。

| 第 2 段階 (リランカー) | 第 1 段階 (埋め込みモデル) |
|---|---|
| jina-reranker-v3.5 | jina-embeddings-v5-text-small |
| jina-reranker-v3 | jina-embeddings-v5-text-small |
| ruri-v3-reranker-310m | ruri-v3-310m |
| sarashina3-rerank | sarashina3-embedding |
| nemotron-3.5-rerank-8b | nemotron-3.5-embed-8b |
| qwen3-reranker-0.6b | qwen3-embedding-0.6b |
| cohere-rerank-v5.0-pro | cohere-embed-v5.0-pro |
| cohere-rerank-v5.0-fast | cohere-embed-v5.0-pro |

### 文脈埋め込みモデル (Contextual Embeddings)

pplx-embed-context-v1 などのモデルは、同一文書に属するチャンク群をまとめて受け取り、各チャンクを周辺文脈込みで埋め込むモデルです。上の表では他のモデルと索引粒度を揃えるため文書単位 (1 文書 = 1 チャンク) で測定しており、この系統の本来の使い方にはあたりません。

参考として、文書を 256 / 128 トークンのチャンクに分割し、文書スコアをチャンクの最大値として集約した場合の Recall@10 を示します。クエリ側は、v1 系では同サイズの pplx-embed-v1 で埋め込み、v2 ではモデル自身の encode_queries を使っています (v2 のクエリに encode を使うと検索品質が低下します)。

| モデル | 文書単位 | 256 トークン | 128 トークン |
|---|---|---|---|
| pplx-embed-v1-4b | 0.8145 | 0.7805 | 0.7506 |
| pplx-embed-context-v1-4b | 0.7862 | 0.7817 | 0.7828 |
| pplx-embed-context-v1-0.6b | 0.7686 | 0.7540 | 0.7471 |
| pplx-embed-v2-context-9b-preview | 0.8075 | 0.8079 | 0.8131 |

### Late Interaction

pplx-embed-v2-late などの Late Interaction (ColBERT 方式) のモデルは、文書とクエリをトークンごとのベクトル列として表現し、MaxSim で採点します。上の表の他の行は 1 文書 = 1 ベクトルのコサイン類似度で検索しているため、検索の仕組みが異なります。

$$\text{score}(q, d) = \sum_{i} \max_{j} (q_i \cdot d_j)$$

| 項目 | 設定 |
|---|---|
| トークンごとの次元 | 128 |
| 1 文書あたりのトークン数 | 平均 258 |
| 索引サイズ | 0.11 GiB (float16) |
