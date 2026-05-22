Once again, very much up for grabs, but here are some thoughts.

## Lexical Search

Lexical search is fundamental and well cemented  
BM25 is still  king in many ways

## Semantic Search

Semantic search is quickly evolving  
It’s not clear how things will play out in Search and LLM space

Hybrid search is the current go-to technique 

* Sometimes it’s more beneficial to present lexical and semantic results separately to the users  
* Mixing them could lead to mixed quality of the results  
* Moving from text to vector is challenging in some languages  
* RRF is the current go-to, but other approaches (normalizing scores) are actively being explored

Selection process for tools and products is sometimes illogical or via “sheep mentality”

Is Solr lagging behind a good thing to allow the domain space to settle in?

Solr being based on Lucene benefits from Amazon’s investment in Elastic  
Can Solr stay up to date with Lucene changes to get the latest cutting-edge features?

Visual language models

* Multi-modal search support  
* Could Solr support multiple vector per document (yes and no)

## Data Exploration / Discovery

Visualize results of the query (ie Kibana for ES)

Clustering results

Carrot is an old contrib module in Solr

Are various “notebook” solutions the way to do this currently? (Superset, Zeppelin)

## Docker / Kubernetes

Too heavyweight / intimidating to learn  
Akka ([https://doc.akka.io/libraries/akka-core/current/typed/guide/modules.html](https://doc.akka.io/libraries/akka-core/current/typed/guide/modules.html))

Community is still trending on move to Kubernetes ecosystem where Operator could see more adoption

## Relevance Testing

There are currently no best practices / solutions

## Stability at Scale

Performance when dealing with clusters with 100s of nodes

