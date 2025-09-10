# Solr Working Vision

* [Why a Vision?](#why-a-vision)
* [What is a Vision?](#what-is-a-vision)
* [What Do We Mean by "Working"?](#what-do-we-mean-by-working)
* ["Working" Process](#working-process)
* [First Iteration Output](#first-iteration-output)
* [What's Next & How to Contribute](#whats-next--how-to-contribute)

## Why a Vision?

Having a shared vision, or at least an ongoing discussion toward one, helps align the Solr community around where the project is headed.

This is good for:

* **Existing community**. To know if it alligns with their objectives and opinions. For example, is it worth contributing more or are their priorities diverging?
* **New people**. When choosing a technology, many people consider not only what it can currently do, but where it's going. For example, the features I'm interested in can be actively developed or look like unmaintained legacies.

---

## What is a Vision?

Terminology can be different to different people, but for the purpose of this discussion, we need to differentiate mission, vision and roadmap:

* **Mission** → Broad, open-ended direction.
  * Example: we're climbing the nicest mountains to enjoy the view.

* **Vision** → A specific, long-term goal: aspirational, measurable, and achievable.
  * Example: we want to climb Kilimanjaro and experience all the climates.

* **Roadmap** → The concrete steps required to reach the vision.
  * Example: we need to find sponsors, buy tickets, train, etc.

---

## What Do We Mean by "Working"?

By “working,” we mean the vision is **iterative, not static**.  

* We almost certainly won’t get it right on the first attempt.  
* Even if we did, the community evolves: users come and go, contributors change, and new requirements emerge (e.g., time-series analysis, vector search, AI agents).

A working vision adapts with the project and its people.

---

## "Working" Process

We propose a progression of reflective questions. For each question:

* Each contributor provides input independently.
* Contributors then meet to discuss inputs towards some consensus.

Questions are divided in categories:

### A. Where Solr is Today <span style="font-weight: normal;">→ Factual</span>

1. 🔍 <span style="color: #1e40af;">**Problem Domain**</span> - What is Solr's (Problem) Domain? What is Search Technology?
2. 📦 <span style="color: #1e40af;">**Current Offering**</span> - What Solr currently offers?
3. 👥 <span style="color: #1e40af;">**Current User Base**</span> - Who is using Solr?
4. ⚖️ <span style="color: #1e40af;">**Competitive Comparison**</span> - How does Solr compare to its alternatives?

### B. Where Things May Be Going <span style="font-weight: normal;">→ Opinionated</span>

5. 🚀 <span style="color: #991b1b;">**Domain Evolution**</span> - In Solr's Problem Domain, what is changing (shifting/evolving/happening)?
6. ⬆️⬇️ <span style="color: #991b1b;">**Attract & Retain / Deter & Disaffect**</span> - What is Solr's current ability to Attract & Retain and current tendency to Deter & Disaffect?

### C. Where We Would Like to See Solr Go <span style="font-weight: normal;">→ Strategic</span>

7. 🔮 <span style="color: #166534;">**Working Vision**</span> - What are the aspirational points on the Horizon worth pursuing?
8. 📈 <span style="color: #166534;">**Roadmap**</span> - What are the important work items that would get us there?

In our first iteration, we used additional ideas and inputs from LLMs to help us with our brainstorming. You'll find them, along with the comments of the working group, in the [working-answers](working-answers) folder.

### Survey

We also asked the community about various items related to 1-6 in a [survey](https://docs.google.com/document/d/1qK3Zkm_T1c_aewrjL3N1k0EqmvA-gl3CdFcpuB0XT0I/edit). We think the survey is also worth iterating on (like the vision does), so that it serves as a good feedback mechanism.

### Package output, get feedback, get contributors

We want to package the answers to 1-8 for each iteration and present them to the community, inviting discussions and further iterations&contributions. It's not the output itself that matters most, but the ongoing effort to allign the community and write down where we are and where we want to go.

---

## First iteration output

Check out our comments for each question in the [working-answers](working-answers) folder.

TL;DR version:

1. Problem domain: Information retrieval, mainly looking at BM25, neural and hybrid search.
2. Current Solr capabilities: A whole lot 🙂
3. Current user base: Somewhat captured in [survey results](https://docs.google.com/document/d/1qK3Zkm_T1c_aewrjL3N1k0EqmvA-gl3CdFcpuB0XT0I/edit?usp=sharing).
4. Competitive comparison: mainly looking at Elasticsearch and OpenSearch, but also others. Error 500 while trying to summarize, too much to say 😅
5. Domain evolution: semantic search, data discovery and visualization, kubernetes, relevance testing, stability at scale.
6. Let's break it down:
    * Attract: pluggability, apache governance, solr operator, flexibility, scalability.
    * Retain: pluggability, hard to migrate, community.
    * Deter: usability, perception of Solr dying, ZK dependency.
    * Disaffect: AI-related features are behind, stability at scale.
7. Vision: Scalable, easy to use, oss swiss-army-knife for the world's most challenging retrieval use cases.
8. Roadmap around the following themes: usability & developer experience, AI & next-gen retrieval, performance & scalability, community & ecosystem.

---

## What's Next & How to Contribute

We’d love your input!  

Ways to contribute:

* Submit PRs or issues in this repo.  
* Comment directly on the [survey document](https://docs.google.com/document/d/1qK3Zkm_T1c_aewrjL3N1k0EqmvA-gl3CdFcpuB0XT0I/edit?usp=sharing).  

Better yet: join the next iteration. The ultimate goal is to ensure this vision reflects the **whole community** and publish the latest version on [solr.apache.org](https://solr.apache.org/).  
