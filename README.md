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
| 3 | Perplexity | [pplx-embed-v2-late-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v2-late-0.6b) | 0.6B | 2026-10 | 0.860 |
| 4 | SB Intuitions | [sarashina3-rerank](https://docs.sarashina.ai/api-reference/rerank) |  | 2026-07 | 0.852 |
| 5 | Cohere | [cohere-embed-v5.0-pro](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.832 |
| 6 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.823 |
| 7 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.821 |
| 8 | SB Intuitions | [sarashina3-embedding](https://docs.sarashina.ai/api-reference/embeddings) |  | 2026-07 | 0.817 |
| 9 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.814 |
| 10 | Perplexity | [pplx-embed-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-v1-4b) | 4B | 2026-02 | 0.814 |
| 11 | Perplexity | [pplx-embed-v2-context-9b-preview](https://huggingface.co/perplexity-ai/pplx-embed-v2-context-9b-preview) | 8.4B | 2026-09 | 0.808 |
| 12 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.806 |
| 13 | Nagoya University | [ruri-v3-reranker-310m](https://huggingface.co/cl-nagoya/ruri-v3-reranker-310m) | 0.31B | 2025-04 | 0.805 |
| 14 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.802 |
| 15 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.802 |
| 16 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.801 |
| 17 | Cohere | [cohere-embed-v5.0-fast](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.797 |
| 18 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.792 |
| 19 | Perplexity | [pplx-embed-context-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-4b) | 4B | 2026-02 | 0.786 |
| 20 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.786 |
| 21 | NVIDIA | [nemotron-3.5-embed-8b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-8B-BF16) | 8.4B | 2026-10 | 0.783 |
| 22 | NVIDIA | [nemotron-3.5-embed-1b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-1B-BF16) | 1.55B | 2026-10 | 0.782 |
| 23 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.780 |
| 24 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.778 |
| 25 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.773 |
| 26 | Perplexity | [pplx-embed-context-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-0.6b) | 0.6B | 2026-02 | 0.769 |
| 27 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.765 |
| 28 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.762 |
| 29 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.761 |
| 30 | Alibaba | [qwen3-reranker-0.6b](https://huggingface.co/Qwen/Qwen3-Reranker-0.6B) | 0.6B | 2025-06 | 0.761 |
| 31 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.756 |
| 32 | Jina AI | [jina-embeddings-v5-omni-small](https://huggingface.co/jinaai/jina-embeddings-v5-omni-small) | 1.74B | 2026-05 | 0.755 |
| 33 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.753 |
| 34 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.751 |
| 35 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.745 |
| 36 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.740 |
| 37 | Jina AI | [jina-embeddings-v5-omni-nano](https://huggingface.co/jinaai/jina-embeddings-v5-omni-nano) | 1.04B | 2026-05 | 0.740 |
| 38 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.738 |
| 39 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.735 |
| 40 | Google | [embeddinggemma-2](https://huggingface.co/google/embeddinggemma-2) | 0.74B | 2026-10 | 0.735 |
| 41 | Jina AI | [jina-reranker-v3.5](https://huggingface.co/jinaai/jina-reranker-v3.5) | 0.6B | 2026-07 | 0.733 |
| 42 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.723 |
| 43 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.719 |
| 44 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.715 |
| 45 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.710 |
| 46 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.706 |
| 47 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.701 |
| 48 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.698 |
| 49 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.683 |
| 50 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.682 |
| 51 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.664 |
| 52 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.660 |
| 53 | Jina AI | [jina-reranker-v3](https://huggingface.co/jinaai/jina-reranker-v3) | 0.6B | 2025-09 | 0.646 |
| 54 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.645 |
| 55 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.642 |
| 56 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.615 |
| 57 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.600 |
| 58 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.566 |
| 59 | Jina AI | [jina-colbert-v2-64](https://huggingface.co/jinaai/jina-colbert-v2-64) | 0.56B | 2024-08 | 0.560 |
| 60 | Jina AI | [jina-colbert-v2](https://huggingface.co/jinaai/jina-colbert-v2) | 0.56B | 2024-08 | 0.557 |
| 61 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.528 |
| 62 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.511 |
| 63 | Yuichi Tateno | [bekko-static-embedding-v1](https://huggingface.co/hotchpotch/bekko-static-embedding-v1) | 0.2B | 2026-09 | 0.482 |
| 64 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.462 |
| 65 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.247 |
| 66 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.199 |
| 67 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.180 |
| 68 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.133 |
| 69 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.130 |

### Precision@10

| Rank | Publisher | Model | Parameter Size | Release Date | Score |
|------|-----------|-------|---------------|-------------|-------|
| 1 | NVIDIA | [nemotron-3.5-rerank-8b](https://huggingface.co/nvidia/Nemotron-3.5-Rerank-8B-BF16) | 8.4B | 2026-10 | 0.204 |
| 2 | Perplexity | [pplx-embed-v2-late-9b](https://huggingface.co/perplexity-ai/pplx-embed-v2-late-9b) | 8.4B | 2026-10 | 0.197 |
| 3 | Perplexity | [pplx-embed-v2-late-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v2-late-0.6b) | 0.6B | 2026-10 | 0.196 |
| 4 | SB Intuitions | [sarashina3-rerank](https://docs.sarashina.ai/api-reference/rerank) |  | 2026-07 | 0.194 |
| 5 | Cohere | [cohere-embed-v5.0-pro](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.191 |
| 6 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.188 |
| 7 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.187 |
| 8 | SB Intuitions | [sarashina3-embedding](https://docs.sarashina.ai/api-reference/embeddings) |  | 2026-07 | 0.187 |
| 9 | Perplexity | [pplx-embed-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-v1-4b) | 4B | 2026-02 | 0.186 |
| 10 | Nagoya University | [ruri-v3-reranker-310m](https://huggingface.co/cl-nagoya/ruri-v3-reranker-310m) | 0.31B | 2025-04 | 0.186 |
| 11 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.185 |
| 12 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.185 |
| 13 | Cohere | [cohere-embed-v5.0-fast](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.184 |
| 14 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.184 |
| 15 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.183 |
| 16 | Perplexity | [pplx-embed-v2-context-9b-preview](https://huggingface.co/perplexity-ai/pplx-embed-v2-context-9b-preview) | 8.4B | 2026-09 | 0.183 |
| 17 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.182 |
| 18 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.181 |
| 19 | NVIDIA | [nemotron-3.5-embed-8b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-8B-BF16) | 8.4B | 2026-10 | 0.181 |
| 20 | NVIDIA | [nemotron-3.5-embed-1b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-1B-BF16) | 1.55B | 2026-10 | 0.180 |
| 21 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.178 |
| 22 | Perplexity | [pplx-embed-context-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-4b) | 4B | 2026-02 | 0.178 |
| 23 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.177 |
| 24 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.177 |
| 25 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.177 |
| 26 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.177 |
| 27 | Perplexity | [pplx-embed-context-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-0.6b) | 0.6B | 2026-02 | 0.175 |
| 28 | Jina AI | [jina-embeddings-v5-omni-small](https://huggingface.co/jinaai/jina-embeddings-v5-omni-small) | 1.74B | 2026-05 | 0.174 |
| 29 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.174 |
| 30 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.174 |
| 31 | Jina AI | [jina-embeddings-v5-omni-nano](https://huggingface.co/jinaai/jina-embeddings-v5-omni-nano) | 1.04B | 2026-05 | 0.174 |
| 32 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.174 |
| 33 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.173 |
| 34 | Alibaba | [qwen3-reranker-0.6b](https://huggingface.co/Qwen/Qwen3-Reranker-0.6B) | 0.6B | 2025-06 | 0.173 |
| 35 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.172 |
| 36 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.172 |
| 37 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.172 |
| 38 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.171 |
| 39 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.171 |
| 40 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.170 |
| 41 | Google | [embeddinggemma-2](https://huggingface.co/google/embeddinggemma-2) | 0.74B | 2026-10 | 0.169 |
| 42 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.167 |
| 43 | Jina AI | [jina-reranker-v3.5](https://huggingface.co/jinaai/jina-reranker-v3.5) | 0.6B | 2026-07 | 0.166 |
| 44 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.163 |
| 45 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.163 |
| 46 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.163 |
| 47 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.159 |
| 48 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.159 |
| 49 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.158 |
| 50 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.158 |
| 51 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.153 |
| 52 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.151 |
| 53 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.148 |
| 54 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.148 |
| 55 | Jina AI | [jina-reranker-v3](https://huggingface.co/jinaai/jina-reranker-v3) | 0.6B | 2025-09 | 0.144 |
| 56 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.142 |
| 57 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.137 |
| 58 | Jina AI | [jina-colbert-v2-64](https://huggingface.co/jinaai/jina-colbert-v2-64) | 0.56B | 2024-08 | 0.132 |
| 59 | Jina AI | [jina-colbert-v2](https://huggingface.co/jinaai/jina-colbert-v2) | 0.56B | 2024-08 | 0.131 |
| 60 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.123 |
| 61 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.121 |
| 62 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.119 |
| 63 | Yuichi Tateno | [bekko-static-embedding-v1](https://huggingface.co/hotchpotch/bekko-static-embedding-v1) | 0.2B | 2026-09 | 0.109 |
| 64 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.108 |
| 65 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.056 |
| 66 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.042 |
| 67 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.038 |
| 68 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.032 |
| 69 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.021 |

### nDCG@10

| Rank | Publisher | Model | Parameter Size | Release Date | Score |
|------|-----------|-------|---------------|-------------|-------|
| 1 | NVIDIA | [nemotron-3.5-rerank-8b](https://huggingface.co/nvidia/Nemotron-3.5-Rerank-8B-BF16) | 8.4B | 2026-10 | 0.811 |
| 2 | Perplexity | [pplx-embed-v2-late-9b](https://huggingface.co/perplexity-ai/pplx-embed-v2-late-9b) | 8.4B | 2026-10 | 0.751 |
| 3 | Perplexity | [pplx-embed-v2-late-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v2-late-0.6b) | 0.6B | 2026-10 | 0.738 |
| 4 | SB Intuitions | [sarashina3-rerank](https://docs.sarashina.ai/api-reference/rerank) |  | 2026-07 | 0.736 |
| 5 | SB Intuitions | [sarashina3-embedding](https://docs.sarashina.ai/api-reference/embeddings) |  | 2026-07 | 0.727 |
| 6 | Google | [gemini-embedding-2-preview](https://docs.cloud.google.com/vertex-ai/generative-ai/docs/models/gemini/embedding-2) |  | 2026-03 | 0.725 |
| 7 | Nagoya University | [ruri-v3-reranker-310m](https://huggingface.co/cl-nagoya/ruri-v3-reranker-310m) | 0.31B | 2025-04 | 0.715 |
| 8 | Perplexity | [pplx-embed-v2-context-9b-preview](https://huggingface.co/perplexity-ai/pplx-embed-v2-context-9b-preview) | 8.4B | 2026-09 | 0.711 |
| 9 | Perplexity | [pplx-embed-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-v1-4b) | 4B | 2026-02 | 0.710 |
| 10 | Tencent | [kalm-embedding-gemma3-12b-2511](https://huggingface.co/tencent/KaLM-Embedding-Gemma3-12B-2511) | 12B | 2025-11 | 0.708 |
| 11 | Google | [gemini-embedding-001](https://developers.googleblog.com/ja/gemini-embedding-available-gemini-api/) |  | 2025-07 | 0.707 |
| 12 | Cohere | [cohere-embed-v5.0-pro](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.704 |
| 13 | SB Intuitions | [sarashina-embedding-v2-1b](https://huggingface.co/sbintuitions/sarashina-embedding-v2-1b) | 1B | 2025-08 | 0.696 |
| 14 | Voyage AI | [voyage-4-large](https://huggingface.co/voyageai/voyage-4-large) |  | 2026-01 | 0.691 |
| 15 | Perplexity | [pplx-embed-context-v1-4b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-4b) | 4B | 2026-02 | 0.689 |
| 16 | Cohere | [cohere-embed-v5.0-fast](https://docs.cohere.com/docs/cohere-embed) |  | 2026-09 | 0.686 |
| 17 | NVIDIA | [nemotron-3.5-embed-8b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-8B-BF16) | 8.4B | 2026-10 | 0.685 |
| 18 | Voyage AI | [voyage-4](https://huggingface.co/voyageai/voyage-4) |  | 2026-01 | 0.681 |
| 19 | Voyage AI | [voyage-4-nano](https://huggingface.co/voyageai/voyage-4-nano) | 0.34B | 2026-01 | 0.666 |
| 20 | Perplexity | [pplx-embed-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-v1-0.6b) | 0.6B | 2026-02 | 0.666 |
| 21 | NVIDIA | [nemotron-3.5-embed-1b](https://huggingface.co/nvidia/Nemotron-3.5-Embed-1B-BF16) | 1.55B | 2026-10 | 0.664 |
| 22 | Google | [embeddinggemma-300m](https://huggingface.co/google/embeddinggemma-300m) | 0.3B | 2025-09 | 0.663 |
| 23 | Alibaba | [qwen3-embedding-8b](https://huggingface.co/Qwen/Qwen3-Embedding-8B) | 8B | 2025-06 | 0.662 |
| 24 | Cohere | [cohere-embed-v4.0](https://docs.cohere.com/docs/cohere-embed) |  | 2025-04 | 0.659 |
| 25 | Perplexity | [pplx-embed-context-v1-0.6b](https://huggingface.co/perplexity-ai/pplx-embed-context-v1-0.6b) | 0.6B | 2026-02 | 0.655 |
| 26 | Amazon | [nova-2-multimodal-embeddings-v1](https://docs.aws.amazon.com/nova/latest/userguide/nova-embeddings.html) |  | 2025-10 | 0.652 |
| 27 | OpenAI | [text-embedding-3-large](https://platform.openai.com/docs/models/text-embedding-3-large) |  | 2024-01 | 0.649 |
| 28 | Jina AI | [jina-reranker-v3.5](https://huggingface.co/jinaai/jina-reranker-v3.5) | 0.6B | 2026-07 | 0.648 |
| 29 | Yuichi Tateno | [japanese-splade-v2](https://huggingface.co/hotchpotch/japanese-splade-v2) | 0.1B | 2024-12 | 0.642 |
| 30 | Microsoft | [harrier-oss-v1-0.6b](https://huggingface.co/microsoft/harrier-oss-v1-0.6b) | 0.6B | 2026-03 | 0.637 |
| 31 | IBM | [granite-embedding-311m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-311m-multilingual-r2) | 0.311B | 2026-04 | 0.637 |
| 32 | Alibaba | [qwen3-reranker-0.6b](https://huggingface.co/Qwen/Qwen3-Reranker-0.6B) | 0.6B | 2025-06 | 0.634 |
| 33 | Alibaba | [qwen3-embedding-4b](https://huggingface.co/Qwen/Qwen3-Embedding-4B) | 4B | 2025-06 | 0.634 |
| 34 | Voyage AI | [voyage-4-lite](https://huggingface.co/voyageai/voyage-4-lite) |  | 2026-01 | 0.633 |
| 35 | Jina AI | [jina-embeddings-v5-omni-small](https://huggingface.co/jinaai/jina-embeddings-v5-omni-small) | 1.74B | 2026-05 | 0.628 |
| 36 | Jina AI | [jina-embeddings-v5-text-small](https://huggingface.co/jinaai/jina-embeddings-v5-text-small) | 0.68B | 2026-02 | 0.628 |
| 37 | Jina AI | [jina-embeddings-v5-text-nano](https://huggingface.co/jinaai/jina-embeddings-v5-text-nano) | 0.24B | 2026-02 | 0.625 |
| 38 | Jina AI | [jina-embeddings-v5-omni-nano](https://huggingface.co/jinaai/jina-embeddings-v5-omni-nano) | 1.04B | 2026-05 | 0.625 |
| 39 | Google | [embeddinggemma-2](https://huggingface.co/google/embeddinggemma-2) | 0.74B | 2026-10 | 0.625 |
| 40 | BAAI | [bge-m3](https://huggingface.co/BAAI/bge-m3) | 0.57B | 2024-02 | 0.620 |
| 41 | Jina AI | [jina-embeddings-v4](https://huggingface.co/jinaai/jina-embeddings-v4) | 4B | 2025-06 | 0.612 |
| 42 | Snowflake | [snowflake-arctic-embed-l-v2.0](https://huggingface.co/Snowflake/snowflake-arctic-embed-l-v2.0) | 0.57B | 2024-12 | 0.600 |
| 43 | Nagoya University | [ruri-v3-310m](https://huggingface.co/cl-nagoya/ruri-v3-310m) | 0.31B | 2025-04 | 0.597 |
| 44 | OpenAI | [text-embedding-3-small](https://platform.openai.com/docs/models/text-embedding-3-small) |  | 2024-01 | 0.590 |
| 45 | IBM | [granite-embedding-278m-multilingual](https://huggingface.co/ibm-granite/granite-embedding-278m-multilingual) | 0.28B | 2024-12 | 0.590 |
| 46 | IBM | [granite-embedding-97m-multilingual-r2](https://huggingface.co/ibm-granite/granite-embedding-97m-multilingual-r2) | 0.097B | 2026-04 | 0.589 |
| 47 | Microsoft | [harrier-oss-v1-270m](https://huggingface.co/microsoft/harrier-oss-v1-270m) | 0.27B | 2026-03 | 0.587 |
| 48 | Jina AI | [jina-embeddings-v3](https://huggingface.co/jinaai/jina-embeddings-v3) | 0.57B | 2024-09 | 0.586 |
| 49 | Alibaba | [qwen3-embedding-0.6b](https://huggingface.co/Qwen/Qwen3-Embedding-0.6B) | 0.6B | 2025-06 | 0.586 |
| 50 | Jina AI | [jina-reranker-v3](https://huggingface.co/jinaai/jina-reranker-v3) | 0.6B | 2025-09 | 0.576 |
| 51 | Microsoft | [multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.571 |
| 52 | Microsoft | [.microsoft-multilingual-e5-large](https://huggingface.co/intfloat/multilingual-e5-large) | 0.56B | 2023-06 | 0.556 |
| 53 | Amazon | [titan-embed-text-v2](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2024-04 | 0.555 |
| 54 | Microsoft | [multilingual-e5-small](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.522 |
| 55 | Microsoft | [.multilingual-e5-small-elasticsearch](https://huggingface.co/intfloat/multilingual-e5-small) | 0.12B | 2023-06 | 0.521 |
| 56 | Amazon | [titan-embed-text-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-embedding-models.html) |  | 2023-09 | 0.495 |
| 57 | Elastic | [BM25 (Kuromoji)](https://www.elastic.co/docs/reference/elasticsearch/plugins/analysis-kuromoji-analyzer) |  |  | 0.494 |
| 58 | NVIDIA | [llama-embed-nemotron-8b](https://huggingface.co/nvidia/llama-embed-nemotron-8b) | 8B | 2025-10 | 0.486 |
| 59 | Jina AI | [jina-colbert-v2-64](https://huggingface.co/jinaai/jina-colbert-v2-64) | 0.56B | 2024-08 | 0.465 |
| 60 | Jina AI | [jina-colbert-v2](https://huggingface.co/jinaai/jina-colbert-v2) | 0.56B | 2024-08 | 0.465 |
| 61 | BizReach | [light-splade-japanese-28m](https://huggingface.co/bizreach-inc/light-splade-japanese-28M) | 0.028B | 2025-11 | 0.411 |
| 62 | BizReach | [light-splade-japanese-14m](https://huggingface.co/bizreach-inc/light-splade-japanese-14M) | 0.014B | 2025-11 | 0.407 |
| 63 | Yuichi Tateno | [bekko-static-embedding-v1](https://huggingface.co/hotchpotch/bekko-static-embedding-v1) | 0.2B | 2026-09 | 0.395 |
| 64 | BizReach | [light-splade-japanese-56m](https://huggingface.co/bizreach-inc/light-splade-japanese-56M) | 0.056B | 2025-11 | 0.356 |
| 65 | Amazon | [titan-embed-image-v1](https://docs.aws.amazon.com/bedrock/latest/userguide/titan-multiemb-models.html) |  | 2023-11 | 0.188 |
| 66 | Elastic | [ELSER](https://www.elastic.co/docs/explore-analyze/machine-learning/nlp/ml-nlp-elser) | 0.11B | 2023-06 | 0.170 |
| 67 | MongoDB | [mdbr-leaf-mt](https://huggingface.co/MongoDB/mdbr-leaf-mt) | 0.023B | 2025-08 | 0.127 |
| 68 | sentence-transformers | [all-minilm-l6-v2](https://huggingface.co/sentence-transformers/all-MiniLM-L6-v2) | 0.023B | 2021-08 | 0.111 |
| 69 | Redis | [langcache-embed-v3-small](https://huggingface.co/redis/langcache-embed-v3-small) | 0.023B | 2025-10 | 0.088 |

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
