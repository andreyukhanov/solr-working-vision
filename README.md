# Solr Working Vision

* [Why a vision?](#why-a-vision)
* [What is a vision?](#what-is-a-vision)
* [What do you mean by "working"?](#what-do-you-mean-by-working)
* ["Working" process](#working-process)
* [First iteration output](#first-iteration-output)
* [What's next? / Contributing](#whats-next--contributing)

## Why a vision?
It's nice to have some consensus - or rather, an ongoing discussion towards a consensus - about where an OSS project is going.

This is good for:
* **Existing community**. To know if it alligns with their objectives and opinions. For example, is it worth contributing more or is it a waste of my time?
* **New people**. When choosing a technology, many people consider not only what it can currently do, but where it's going. For example, the features I'm interested in can be actively developed or look like unmaintained legacies.

## What is a vision?
Terminology can be different to different people, but for the purpose of this discussion, we need to differentiate mission, vision and roadmap:
* A **mission** is the general direction and is often open-ended. E.g., we're climbing the nicest mountains to enjoy the view.
* A **vision** is a long-term goal, achievable and measurable, but still concise and aspirational. E.g., we want to climb Kilimanjaro and experience all the climates.
* A **roadmap** is the list of detailed steps that get us to the vision. We need to find sponsors, buy tickets, train, etc.

## What do you mean by "working"?
It means it's not static. We want **iterations**. Because:
* It's **unlikely to get it right on the first try**. That is, have a vision that represents the Solr community as a whole.
* Even if we do, things change: both the community itself (users and contributors come and go) and its requirements (e.g., time-series analysis, vector search, agents...).

## "Working" process
We propose a progression of reflective questions. For each question:
* Each contributor provides input independently.
* Contributors then meet to discuss inputs towards some consensus.

Questions are divided in categories:

### A. Where Solr is Today <span style="font-weight: normal;">→ Factual</span>
1. 🔍 <span style="color: #1e40af;">**Problem Domain**</span> - What is Solr's (Problem) Domain? What is Search Technology?
2. 📦 <span style="color: #1e40af;">**Current Offering**</span> - What Solr currently offers?
3. 👥 <span style="color: #1e40af;">**Current User Base**</span> - Who is using Solr?
4. ⚖️ <span style="color: #1e40af;">**Competitive Comparison**</span> - How does Solr compare to its alternatives?
### B. Where things may be going <span style="font-weight: normal;">→ Opinionated</span>
5. 🚀 <span style="color: #991b1b;">**Domain Evolution**</span> - In Solr's Problem Domain, what is changing (shifting/evolving/happening)?
6. ⬆️⬇️ <span style="color: #991b1b;">**Attract & Retain / Deter & Disaffect**</span> - What is Solr's current ability to Attract & Retain and current tendency to Deter & Disaffect?
### C. Where we would like to see things go <span style="font-weight: normal;">→ Strategic</span>
7. 🔮 <span style="color: #166534;">**Working Vision**</span> - What are the aspirational points on the Horizon worth pursuing?
8. 📈 <span style="color: #166534;">**Roadmap**</span> - What are the important work items that would get us there?

In our first iteration, we used additional ideas and inputs from LLMs to help us with our brainstorming. You'll find them, along with the comments of the working group, in the [working-answers](working-answers) folder.

#### Survey
We also asked the community about various items related to 1-6 in a [survey](https://docs.google.com/document/d/1qK3Zkm_T1c_aewrjL3N1k0EqmvA-gl3CdFcpuB0XT0I/edit). We think the survey is also worth iterating on (like the vision does), so that it serves as a good feedback mechanism.

#### Package output, get feedback, get contributors
We want to package the answers to 1-8 for each iteration and present them to the community, inviting discussions and further iterations&contributions. It's not the output itself that matters most, but the ongoing effort to allign the community and write down where we are and where we want to go.

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

## What's next? / Contributing
If you have ANY feedback, feel free to add it:
* PRs, issues to this repo.
* Comments to the [survey GDoc](https://docs.google.com/document/d/1qK3Zkm_T1c_aewrjL3N1k0EqmvA-gl3CdFcpuB0XT0I/edit?usp=sharing).

Ideally, participate to the next iteration or somehow signal your position. We'd like to make sure that this working vision is representative enough for the whole community, with the end goal of putting [the latest version] on [solr.apache.org](https://solr.apache.org/) somewhere.
