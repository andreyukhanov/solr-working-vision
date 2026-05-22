# Roadmap

*“Apache Solr: The scalable, easy-to-use, OSS swiss-army-knife for the world’s most challenging retrieval use cases.”*

## **Theme 1: Usability & Developer Experience**

**Vision:** *Easy to Start → Easy to Use → Easy to Master*

**2025-2026**

* Revamp developer on-ramp: quickstarts, Docker/K8s templates, Operator examples.  
* Expand V2 API docs and examples.  
* Enhance (new?) Admin UI with data exploration, query visualization, and basic relevance tuning (incl. RRF, hybrid search).  
* Publish “How to do X in Solr” guides.

**2027**

* Unify overlapping features (faceting, highlighting).  
* Deliver next-gen Admin UI: relevance experiments, dashboards, KPIs.  
* Guided schema & query tuning wizards.

**2028**

* Kibana-class UI parity: full visualization, dashboards, and self-service SolrCloud management.  
* Team workspaces and guided workflows for tuning and exploration.

---

## **Theme 2: AI & Next-Gen Retrieval**

**Vision:** *Feature parity and leadership in AI retrieval (vectors, RAG, hybrid).*

**2025-2026**

* Close Lucene vector gap (HNSW, ANN, hybrid).  
* Ship hybrid vector+keyword search as a default.  
* Add pluggable rerankers (e.g. BM25+Vector, LTR).  
* Publish competitive benchmarks vs. ES/OS (100M+ embeddings).

**2027**

* Reference RAG pipelines (ingestion → embedding → query rewrite → rerank).  
* Support Bring-Your-Own embedding/reranker models.  
* Optimizations for billion-scale vector datasets.  
* Provide evaluation harnesses for search quality benchmarking.

**2028**

* Native RAG pipelines GA: embeddings, query rewriting, document enrichment.  
* Model registry for embeddings/rerankers.  
* Hybrid-first ranking enabled out-of-the-box.  
* Public leaderboards showing Solr’s performance vs. Elasticsearch/OpenSearch.

---

## **Theme 3: Performance & Scalability**

**Vision:** *The most scalable OSS retrieval system, cloud-native and cost-efficient.*

**2025-2026**

* Continuous benchmarking framework, published openly.  
* Fix scalability issues (Overseer, cluster state).  
* Solr Operator: auto-scaling and resilience enhancements.

**2027**

* Stateless search nodes.  
* Compute–storage separation to enable independent scaling.  
* Smarter caching and query routing.

**2028**

* Showcase 10B+ document/vector benchmarks.  
* Autoscale SLOs with performance/cost calculators.  
* Advanced ingestion scaling: streaming, real-time pipelines.

---

## **Theme 4: Community & Ecosystem**

**Vision:** *A vibrant, growing, and engaged Solr ecosystem.*

**2025-2026**

* Annual *State of Search / Solr Survey*.  
* Launch roadmap/vision microsite with ongoing updates.  
* Contributor mentorship program to onboard new developers.

**2027**

* Global Solr meetups \+ community conference.  
* Solution blueprints (ecommerce, enterprise search, log analytics).  
* Partnerships for connectors (BI tools, embeddings).

**2028**

* Increased committer diversity and participation.  
* Contributor recognition program.  
* Long-term sponsorship for AI and UI initiatives.

