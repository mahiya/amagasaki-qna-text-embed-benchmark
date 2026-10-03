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
| 1 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.823 |
| 2 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.821 |
| 3 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.814 |
| 4 | Perplexity | [pplx-embed-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-v1-4b) | 4B | 2026-02 | 0.814 |
| 5 | Perplexity | [pplx-embed-v2-context-9b-preview](https://huggingface.co/perplexity-ai/pplx-embed-v2-context-9b-preview) | 8.4B | 2026-09 | 0.808 |
| 6 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.806 |
| 7 | Nagoya University | [ruri-v3-reranker-310m](https://huggingface.co/cl-nagoya/ruri-v3-reranker-310m) | 0.31B | 2025-04 | 0.805 |
| 8 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.802 |
| 9 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.802 |
| 10 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.792 |
| 11 | Perplexity | [pplx-embed-context-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-4b) | 4B | 2026-02 | 0.786 |
| 12 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.780 |
| 13 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.778 |
| 14 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.773 |
| 15 | Perplexity | [pplx-embed-context-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-0.6b) | 0.6B | 2026-02 | 0.769 |
| 16 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.765 |
| 17 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.765 |
| 18 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.762 |
| 19 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.761 |
| 20 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.756 |
| 21 | Jina AI | [jina-embeddings-v5-omni-small](https://huggingface.co/jinaai/jina-embeddings-v5-omni-small) | 1.74B | 2026-05 | 0.755 |
| 22 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.753 |
| 23 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.748 |
| 24 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.745 |
| 25 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.740 |
| 26 | Jina AI | [jina-embeddings-v5-omni-nano](https://huggingface.co/jinaai/jina-embeddings-v5-omni-nano) | 1.04B | 2026-05 | 0.740 |
| 27 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.738 |
| 28 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.735 |
| 29 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.734 |
| 30 | Jina AI | [jina-reranker-v3.5](https://huggingface.co/jinaai/jina-reranker-v3.5) | 0.6B | 2026-07 | 0.733 |
| 31 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.723 |
| 32 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.719 |
| 33 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.715 |
| 34 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.710 |
| 35 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.706 |
| 36 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.698 |
| 37 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.683 |
| 38 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.682 |
| 39 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.673 |
| 40 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.664 |
| 41 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.660 |
| 42 | Jina AI | [jina-reranker-v3](https://huggingface.co/jinaai/jina-reranker-v3) | 0.6B | 2025-09 | 0.646 |
| 43 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.645 |
| 44 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.642 |
| 45 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.615 |
| 46 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.600 |
| 47 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.566 |
| 48 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.528 |
| 49 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.511 |
| 50 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.462 |
| 51 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.247 |
| 52 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.199 |
| 53 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.180 |
| 54 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.133 |
| 55 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.130 |

### Precision@10

| Rank | Publisher | Model | Parameter Size | Release Date | Score |
|------|-----------|-------|---------------|-------------|-------|
| 1 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.188 |
| 2 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.187 |
| 3 | Perplexity | [pplx-embed-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-v1-4b) | 4B | 2026-02 | 0.186 |
| 4 | Nagoya University | [ruri-v3-reranker-310m](https://huggingface.co/cl-nagoya/ruri-v3-reranker-310m) | 0.31B | 2025-04 | 0.186 |
| 5 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.185 |
| 6 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.185 |
| 7 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.183 |
| 8 | Perplexity | [pplx-embed-v2-context-9b-preview](https://huggingface.co/perplexity-ai/pplx-embed-v2-context-9b-preview) | 8.4B | 2026-09 | 0.183 |
| 9 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.182 |
| 10 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.181 |
| 11 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.178 |
| 12 | Perplexity | [pplx-embed-context-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-4b) | 4B | 2026-02 | 0.178 |
| 13 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.177 |
| 14 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.177 |
| 15 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.177 |
| 16 | Perplexity | [pplx-embed-context-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-0.6b) | 0.6B | 2026-02 | 0.175 |
| 17 | Jina AI | [jina-embeddings-v5-omni-small](https://huggingface.co/jinaai/jina-embeddings-v5-omni-small) | 1.74B | 2026-05 | 0.174 |
| 18 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.174 |
| 19 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.174 |
| 20 | Jina AI | [jina-embeddings-v5-omni-nano](https://huggingface.co/jinaai/jina-embeddings-v5-omni-nano) | 1.04B | 2026-05 | 0.174 |
| 21 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.174 |
| 22 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.173 |
| 23 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.172 |
| 24 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.172 |
| 25 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.172 |
| 26 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.171 |
| 27 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.170 |
| 28 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.170 |
| 29 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.168 |
| 30 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.167 |
| 31 | Jina AI | [jina-reranker-v3.5](https://huggingface.co/jinaai/jina-reranker-v3.5) | 0.6B | 2026-07 | 0.166 |
| 32 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.163 |
| 33 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.163 |
| 34 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.163 |
| 35 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.162 |
| 36 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.159 |
| 37 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.158 |
| 38 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.158 |
| 39 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.153 |
| 40 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.152 |
| 41 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.151 |
| 42 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.148 |
| 43 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.148 |
| 44 | Jina AI | [jina-reranker-v3](https://huggingface.co/jinaai/jina-reranker-v3) | 0.6B | 2025-09 | 0.144 |
| 45 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.142 |
| 46 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.137 |
| 47 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.123 |
| 48 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.121 |
| 49 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.119 |
| 50 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.108 |
| 51 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.056 |
| 52 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.042 |
| 53 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.038 |
| 54 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.032 |
| 55 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.021 |

### nDCG@10

| Rank | Publisher | Model | Parameter Size | Release Date | Score |
|------|-----------|-------|---------------|-------------|-------|
| 1 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.725 |
| 2 | Nagoya University | [ruri-v3-reranker-310m](https://huggingface.co/cl-nagoya/ruri-v3-reranker-310m) | 0.31B | 2025-04 | 0.715 |
| 3 | Perplexity | [pplx-embed-v2-context-9b-preview](https://huggingface.co/perplexity-ai/pplx-embed-v2-context-9b-preview) | 8.4B | 2026-09 | 0.711 |
| 4 | Perplexity | [pplx-embed-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-v1-4b) | 4B | 2026-02 | 0.710 |
| 5 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.708 |
| 6 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.707 |
| 7 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.696 |
| 8 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.691 |
| 9 | Perplexity | [pplx-embed-context-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-4b) | 4B | 2026-02 | 0.689 |
| 10 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.681 |
| 11 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.666 |
| 12 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.666 |
| 13 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.663 |
| 14 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.659 |
| 15 | Perplexity | [pplx-embed-context-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-0.6b) | 0.6B | 2026-02 | 0.655 |
| 16 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.652 |
| 17 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.649 |
| 18 | Jina AI | [jina-reranker-v3.5](https://huggingface.co/jinaai/jina-reranker-v3.5) | 0.6B | 2026-07 | 0.648 |
| 19 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.642 |
| 20 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.637 |
| 21 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.637 |
| 22 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.633 |
| 23 | Jina AI | [jina-embeddings-v5-omni-small](https://huggingface.co/jinaai/jina-embeddings-v5-omni-small) | 1.74B | 2026-05 | 0.628 |
| 24 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.628 |
| 25 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.625 |
| 26 | Jina AI | [jina-embeddings-v5-omni-nano](https://huggingface.co/jinaai/jina-embeddings-v5-omni-nano) | 1.04B | 2026-05 | 0.625 |
| 27 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.621 |
| 28 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.620 |
| 29 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.618 |
| 30 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.612 |
| 31 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.600 |
| 32 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.597 |
| 33 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.590 |
| 34 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.590 |
| 35 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.589 |
| 36 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.587 |
| 37 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.586 |
| 38 | Jina AI | [jina-reranker-v3](https://huggingface.co/jinaai/jina-reranker-v3) | 0.6B | 2025-09 | 0.576 |
| 39 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.571 |
| 40 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.563 |
| 41 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.556 |
| 42 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.555 |
| 43 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.522 |
| 44 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.521 |
| 45 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.495 |
| 46 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.494 |
| 47 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.486 |
| 48 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.411 |
| 49 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.407 |
| 50 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.356 |
| 51 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.188 |
| 52 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.170 |
| 53 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.127 |
| 54 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.111 |
| 55 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.088 |

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

### 文脈埋め込みモデル (Contextual Embeddings)

pplx-embed-context-v1 などのモデルは、同一文書に属するチャンク群をまとめて受け取り、各チャンクを周辺文脈込みで埋め込むモデルです。上の表では他のモデルと索引粒度を揃えるため文書単位 (1 文書 = 1 チャンク) で測定しており、この系統の本来の使い方にはあたりません。

参考として、文書を 256 / 128 トークンのチャンクに分割し、文書スコアをチャンクの最大値として集約した場合の Recall@10 を示します。クエリ側は、v1 系では同サイズの pplx-embed-v1 で埋め込み、v2 ではモデル自身の encode_queries を使っています (v2 のクエリに encode を使うと検索品質が低下します)。

| モデル | 文書単位 | 256 トークン | 128 トークン |
|---|---|---|---|
| pplx-embed-v1-4b | 0.8145 | 0.7805 | 0.7506 |
| pplx-embed-context-v1-4b | 0.7862 | 0.7817 | 0.7828 |
| pplx-embed-context-v1-0.6b | 0.7686 | 0.7540 | 0.7471 |
| pplx-embed-v2-context-9b-preview | 0.8075 | 0.8079 | 0.8131 |
