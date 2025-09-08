  
(JG \- Creating headings for the 4 “categories”.  I’ve moved the previous content on this page down a bit, as it looked more like TODO items and things we can do to improve than analysis)

**Attract**

- Pluggability: Solr is very customizable (JG: more so than competitors?)  
- Apache Governance and OSS Pedigree  
  - Do potential users still see Solr as unique here, or are folks that value this starting to consider OpenSearch as viable in this category as well? (RG) I'd say that most people use OpenSearch because it's a no-strings-attached ES, and not because they believe it's truly OSS. Sure, it belongs to Linux Foundation now, but I don't think people feel like they can have any control over its direction. Which is where Solr is different
- (RG) Solr Operator may be a massive opportunity here. Everyone and their mom uses k8s (see survey), and Solr is the only community incentivised to build a feature-complete k8s integration. And I think that right now it’s the best k8s integration (compared to competitors). Plus, the customizability is an advantage here in the long term.  
- (RG but really CB) Solr is the most flexible search engine out there (i.e. it fits more use-cases than ES/OS/Vespa though it may not be the best at all of them). So as a swiss-army knife for research done by data scientists, it can be very good \=\> new (and growing\!) market  
- (CB) I only have 3 thoughts on this front:  
  - User Interface, User Interface and User Interface  
  - Working Vision  
  - Scalability  
- **\#1 Expand \- the Relevance of Search**  
  - Who it is relevant to   
  - How it is relevant to them  
  - Expand the Search Technology well beyond the retrieval of documents and into the actions users can take upon it  
- **\#2 Evolve \- the Ability and Nature of Scaling Data**  
  - From speed and ease of ingestion to pushing the envelope of how data can scale

**Retain**

- Pluggability \- once users create custom Solr plugins, there’s an additional entrenchment factor  
- General Entrenchment \- migrating production systems is hard, and Solr is close enough to competitors perf, feature-wise to disincentivize such a big effort  
- (RG) Community that can help you now and wrote a crapton of tutorials in the past  
- Don’t get behind on Lucene APIs  
- Have a Working Vision that ties to a Working Roadmap that is easily accessed and understood

**Deter**

- Usability \- Solr lags behind others in APIs, client availability, “Getting Started Experience”, etc.  
- “Hearts and Minds” \- though there’s a kernel of truth to it, [the reports of Solr’s death are greatly exaggerated](https://www.thisdayinquotes.com/2018/06/reports-of-mark-twains-quip-about-his-death-are-greatly-misquoted/#:~:text=According%20to%20a%20widely%2Drepeated,%E2%80%A6have%20been%20greatly%20exaggerated.%E2%80%9D).  But the perceptionis damaging on its own.  Folks see developer evangelism for Elastic and OpenSearch that dwarfs that around Solr, and their minds are half made up already.  
  - (RG) I think this is by far the biggest problem. Even hardcore Solr peeps don’t recommend Solr to their clients because of this.  
- (RG) Ecosystem, especially visualization tools (e.g. as I’m looking to build integrations for Vespa, everyone supports ES, very few support Solr).  
- Ops / Deployment Complexity \- ZooKeeper is an additional maintenance burden

**Disaffect**

- (RG) AI-related features are behind. That’s the number one reason I see people going from Solr to Vespa.  
- (RG) stability at scale \- main reason I saw people move to ES/OS

##  Things that may help 

Plugin points

- Documentation: list them, add tutorials  
- Promote packages

Usability, for sure 🙂

Make it clear that Solr is truly OSS? 🙂

“How to customize Solr” \- Add to User Guide.  
	  
Plug-in / Package Ecosystem

Integrations (maybe with coding tools, we can add integrations to important ETL tools, E-commerce frameworks, etc.). Anything that could rival Kibana here?

Solr conference:

- Bring community together, make it easier to organize  
- Market that Solr is alive :)

Maybe Community Over Code is that conference?  
