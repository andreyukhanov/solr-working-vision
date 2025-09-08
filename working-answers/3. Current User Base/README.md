This is mostly dealt with in the Search Survey. More details about it [here](https://docs.google.com/document/d/1qK3Zkm_T1c_aewrjL3N1k0EqmvA-gl3CdFcpuB0XT0I/edit?usp=sharing)

## 2025 Search Survey TL;DR
* **Frequently used features**: mostly relevance-related (e.g. vector search, re-ranking), some naturally with operations (e.g. collect metrics), with two other stand-outs:
  * Admin UI. Solr has this as an entry-point, but users of other search techs also use equivalent UIs.
  * Nested documents and joins. Almost half of the respondents need to define relations between documents.
* **Deployment**: most people run small-scale, multi-node setups, but there are a lot of organizations with large scale (e.g. 50+ nodes) and a big chunk (1/3) are using Kubernetes. Correlates with improvements areas, where many users selected "scalability & performance".
* **Improvement areas**: "AI & Semantic search" is the first one by far, followed by the related topic of "relevance tuning". Usability-related topics were also selected a lot, including config complexity, documentation and visualization tools.
* Many people want to get involved, and it looks like the main barriers are funding and ease of contribution. Which are somewhat correlated: if it's easier to contribute, less funding is needed to do so.
* Sample biases:
  * **Role and company**: mostly engineers, many from large organizations.
  * **Use-case**: mostly "pure search" like E-commerce, Enterprise search.
  * **Search engine**: Solr is best represented, Elasticsearch, OpenSearch have good response rates, and we have decent signal for standalone Lucene and Vespa.