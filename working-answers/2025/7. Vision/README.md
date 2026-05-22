**Radu:**  
*I'd push Solr to be a "Scalable OSS swiss-army-knife for retrieval". Basically, push further what Solr is already good at, with the intention of making it its own category. That's what I've learned from marketing folks: if you want to win, be alone in your category :smile: In Solr's case, there's nothing out there with the Solr's flexibility and I'm not aware of anything that pushes in that direction, either.*

Concretely, how this "push" looks in my mind (in no particular order):

* Enhance usability, especially for developers (again, something Solr is already good at). The first thing here might be official tutorials for writing all sorts of plugins.  
* Get up to speed with Lucene vector stuff (so that you're not missing tools in that knife)  
* Enhance the Solr Operator, so that people easily\&reliably deploy on k8s: once again, Solr is the best at this right now.  
* Enhance Solr Admin (or write a new UI, or convince Christopher to donate his Navigator, or...) so that it's better at exploring data (i.e. building queries and visualizations).

**Christopher:**

1\. *Actively exploring the Leading Edge*  
      Acting where people are actively looking for new capabilities \- It can sound commonplace, but it is also a way of keeping current and attracting input and assistance. At the very least, clearly communicating what could be done and evolving the message around the progress being made.

2\. *Actively pushing the User Experience*  
    While performance capabilities may establish credibility, it is the individual user experience that can establish commitment and satisfaction. The first half of the experience is the ease of the on-ramp; the second half is the richness of user interaction.

3\. *Expanding the relevance of Search*  
  Who it is relevant to  
  How it is relevant to them  
  Expand the Search Technology well beyond the retrieval of documents and into the actions users can take upon it

4\. *Evolve the ability and nature of Scaling Data*  
    From speed and ease of ingestion to pushing the envelope of how data can scale

5\. *Engaging the Community and treating Communication is a key aspect facilitating progress*  
  Annual Survey of Search Technology  
  Living Working Vision process with intuitive Roadmap  
  Stratified Communication  
  Newcomer \-\> earn your level of engagement  
  Ongoing tactical issues \-\> Jira Tickets  
  Evolving Longer-term Issues \-\> trends, direction, evolution"

**Jason:**  
*"Easy to Start, Easy to Use, Easy to Master"*

* "Easy to Start"  
  * \[Already There\] Solr's licensing, longevity, and governance make it an easy option that even the most cautious orgs can consider  
  * \[Needs Work\] A strong library of "Getting Started" materials helps users start their Solr journey with confidence.  
* “Easy to Use”  
  * \[Already There\] Solr's Reference Guide isn't just copious, but carefully curated.  Documentation quality is high, and the open community helps answer any inevitable gaps.  
  * \[Needs Work\] Solr's APIs and query language make it easy to understand and reason about, and its selection of clients makes it easy for users to use from any language or environment.  
* “Easy to Master”  
  * \[Needs Work\] Solr's wide array of extension points and integrations makes it easy to integrate into any corporate environment; easing auth, search and indexing customization, visualization, etc.

**Andrey:**  
Feature Parity / AI

* Staying up to date on the latest developments. Falling behind discourages people from trying / using Solr for new development, specifically RAG/AI related  
* Performance of vector search at scale. Many of the vector DBs makes claims that they scale better at hundreds of millions or billions of embedding compared to Solr and other “standard search engines”

Usability 

* Streamlining of APIs (V2), including documentation and examples.  
* Getting started. Make it easy as possible to run Solr for the first time. This includes dependency on ZooKeeper for SolrCloud, which can be daunting.   
* Tutorials. Solr has lots of features. Most used ones have examples or tutorials floating around, but more niche ones require users to figure out how to use them on their own  
* Documentation. Similar to above Solr ref guide covers majority of the features, but some of the more niche ones can use more details  
* UI. There are lots of “user wants” that go into this. Data visualization and exploration, relevance tuning and experimentation, built-in metrics and KPIs, self-service SolrCloud management, etc

Performance / Scalability 

* Solr scales very well up to a certain point (you can say the same for any technology). Many other search engines advertise their improvements in scale. Solr doesn’t do this well at the moment, due to lack of benchmarking that can be run on consistent basis  
* Some of Solr’s architectural designs can become a challenge at scale. For example, Overseer and Clusterstate.json management  
* Separation of compute and storage. With current design, Solr has to scale with both. ES and OpenSearch allow you to scale compute and storage separately, which can be advantageous and more cost efficient for large use cases

Community 

* This is one is challenging for me as other search engines have dedicated entities driving the direction, marketing, and engagement. This does perhaps take away a little from the OSS aspect of it, but it does bring those products front and center into the spotlight.   
* We know lots of folks use Solr, but many are passively involved in the community. How do we get folks to become more active?  
* Meetups and conferences. Similar to point one, these sort of things can help raise awareness and community participation

Alessandro:  
In general, I’m in agreement with all the other points of view, some additions/rephrases from my side:  
**\[Catching up with Lucene\]- in progress**  
Since the split happened, we can clearly see a difficulty in staying up to date with Lucene's new features (especially vector-search-related).  
This should be a priority; thanks to some sponsorship, we are closing the gap in regards to vector search, but this should be a continuous effort.  
A nice initiative is the vector search sub-group, which is also helping.  
**\[AI new features\] \- TO DO**  
A lot of new features can be added directly in Solr, and we are currently lacking the sponsorship/man-power to do it at the pace I would love to see (RAG, LLM integrations for query/document enrichment)  
**\[Usability\] \- in progress**  
Aside from general improvements, I feel we should dedicate a more targeted initiative to simplify some of the “too many ways of doing the same thing”, I know that flexibility is great, but I’m pretty sure that we can unify some of the approaches or deprecate others nowadays (see faceting, highlighting, etc.)  
**\[Benchmarks\]- TO DO**  
Having dedicated public online benchmarks such as the Lucene ones, can be a very nice addition to give new users confidence in Solr good scalability capabilities.  
**\[UI\] \- TO DO**  
I think that inevitably Solr is lacking of a UI up to the standard that users expect from a modern search engine in terms of data exploration.  
The solr admin is decent, but having a Kibana equivalent I suspect is a must.  
This is a challening one as it would take a lot of effort to do it (and I don’t see this easy to happen soon)

## Asynchronous Iteration

\[Written by Jason alone as a starting point for iteration\]

### Brainstorming

While we all chose different things to emphasize, there’s a lot of commonality between our individually-created visions:

* Scaling  
  * Radu: “**Scalable** OSS swiss-army-knife…”  
  * Christopher “*Evolve the ability and nature of **Scaling Data***”  
* Flexibility / “Jack of All Trades”  
  * Radu: “*Scalable OSS **swiss-army-knife…***”  
  * Jason “Solr’s **wide array of extension points and integrations** make it easy…”  
* Usability  
  * Radu: “**Enhance usability**, especially for developers…”  
  * Christopher: “it is **the individual user experience** that can establish commitment and satisfaction”  
  * Jason: “***Easy to Start, Easy to Use, Easy to Master**”*

So these commonalities are really what a “Vision” would draw out IMO.

### Tagline

Radu’s tagline seems like the best starting point, since it already highlights two of the three common areas (“Usability” being the missing piece).  Christopher also expressed some hesitation that the “swiss-army-knife” language brings in the connotation of it being for “toy” usecases (though maybe the presence of “Scalable” already handles that?)

With that in mind, what do we think about:

“The scalable, easy-to-use, OSS swiss-army-knife for the world’s most challenging retrieval use-cases”

Or perhaps…

The easy-to-use, community-first, swiss-army-knife for the world’s largest retrieval use-cases.

### “More Explanation”

Of course, we need more than a tagline \- the Vision needs to be detailed and concrete enough that folks can translate it in their minds into potential roadmap items.  So given the commonalities above, I’d propose something like the following:

* “Scalable”  
  * Solr pushes the envelope of how data can scale \- it’s suitable for the world’s smallest use-cases, and the largest.  
  * Solr’s tight integration with Kubernetes via the Solr Operator allows it to scale with ease in the environments used by today’s developers.  
* “Easy to Pick, Easy to Use”  
  * Solr's licensing, longevity, and governance make it an easy option that even the most cautious orgs can consider  
  * Solr's APIs and query language make it easy to understand and reason about, and its selection of clients makes it easy for users to integrate with, whatever language their application uses.  
* “Swiss Army Knife”  
  * Solr’s strength is its variety.  If your team needs an engine that can handle ecommerce search, enterprise search, and everything in between \- pick Solr.   
  * Solr’s wide array of extension points and integrations makes it easy to integrate  into any corporate environment; easing auth, search and indexing customization, visualization, etc.