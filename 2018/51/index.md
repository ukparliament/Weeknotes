## 2018 Week 51

### The end of an era

On Friday it was announced that further development on the data platform will come to a halt in the new year. So this is the last missive from your parliamentary data mouses. We've had a decent run. And, I think, spent three years doing some of the best work in the public sector. There is a good deal to be proud of and some regret we can't continue.

### Use hypertext to subvert hierarchies

The final jigsaw piece of [Anya](https://twitter.com/bitten_)'s work with the Procedural Publishing Unit clipped into place this week when [Monday's House of Commons Order Paper was the first in history to contain actual anchor links to business items](https://twitter.com/bitten_/status/1074598664549613569). Like how the web works. It all [seemed](https://twitter.com/PennyYoungHoC/status/1074736441408806912) [to](https://twitter.com/LucindaMaer/status/1074739495705198593) [go](https://twitter.com/estrangeirada/status/1074932310494117888) [down](https://twitter.com/andyfacts/status/1074939377485254656) [rather](https://twitter.com/timlb/status/1074952201829679105) [well](https://twitter.com/hamlynm1/status/1074760576281272322). Though we would like to point out, [contrary to some rumours](https://twitter.com/tomskitomski/status/1074933711492300800), we've long been aware of the [power of hypertext](http://www.cluetrain.com/). It means we've now covered off [the Order Paper](https://publications.parliament.uk/pa/cm201719/cmagenda/ob181217.htm#20181217-7), [Future Business](https://publications.parliament.uk/pa/cm201719/cmagenda/fb181220.htm#20181220-63) and [Votes and Proceedings](https://publications.parliament.uk/pa/cm201719/cmvote/181220v01.html#anchor-8). Work like this is important. No order was dispatched from on high. Just some people chatting and exploring ways to make a thing just that little bit better. Somewhere between self evident and profound. Top work Anya and Mark.

### Community

Way back in September, team:[Samu](https://twitter.com/langsamu) headed off to [an Ontotext meetup](https://twitter.com/langsamu/status/1075474136204537856) to chat about ontology engineering, the architecture of our Open Linked Data Platform, the tooling around it, it's readiness for production workloads, monitoring and all other things related to building resilient semantic web infrastructure. Wojciech, Mike, [Chris](https://twitter.com/chrisalcockdev) and [Matthieu](https://twitter.com/cognithive) all had their say. Ontotext have now [published a video from the event](https://www.youtube.com/watch?v=2WvgE34Sqjc) which is a pretty good record of three years of solid work. We suspect Samu might be proud of the team he built. We're proud of it too.

Elsewhere our Samu was on the receiving end of a [Twitter question](https://twitter.com/atomless/status/1073220286651252736) about tallying counts from the [data.parliament divisions API](http://lda.data.parliament.uk/commonsdivisions/id/105056.json). He went in with a reply that managed to pull off a [very nice triple negative](https://twitter.com/langsamu/status/1073216701729308672). Then [Michael](https://twitter.com/fantasticlife) chipped in with [something a little more pragmatic](https://twitter.com/fantasticlife/status/1073231241137283077). And [Dan](https://twitter.com/dasbarrett) finished off by [redirecting them to the real experts](https://twitter.com/UKParliData/status/1073224382976286720).

Tuesday saw Anya, Samu, Robert, Wojciech, Mike, Matthieu, [Jianhan](https://twitter.com/jianhanzhu), [Oli](https://twitter.com/olihawkins) and Michael meet with [Oliver Heath](https://twitter.com/olhe), a professor of politics at [Royal Holloway](https://www.royalholloway.ac.uk/). Oliver’s working on an [ESRC](https://esrc.ukri.org/) funded project to map census data onto constituency boundaries from 1851 to 2018 and is looking for organisations to partner. We volunteered to help where possible. But that was when we still had a data platform. Which we no longer do.

### One world, one web, one team

Robert and Michael had another meeting with [Sarah](https://twitter.com/SarahPurssell), Simon and Laurence about progress with the [formal body](https://ukparliament.github.io/ontologies/formal-body/formal-body-ontology.html), [formal body affiliation](https://ukparliament.github.io/ontologies/formal-body-affiliation/formal-body-affiliation-ontology.html) and [business item](https://ukparliament.github.io/ontologies/business-item/business-item-ontology.html) models. All in the general direction of trying to help build web pages for committees. Although they're not completely convinced why. They're still in search of a label for the overlapping group of groups that covers formal bodies, [answering bodies](https://ukparliament.github.io/ontologies/question-and-answer/question-and-answer-ontology.html#d4e543), [laying bodies](https://ukparliament.github.io/ontologies/laying/laying-ontology.html#d4e308) and government organisations. Again they ask why.

On Tuesday, Anya, Robert and Michael popped across St James's Park to Lego castle that houses the [Parliamentary Computational Section](https://pds.blog.parliament.uk/) for a chat with [Bex](https://twitter.com/rklappleyard), Christine and [Matt](https://twitter.com/mattrayner). Together they attempted to persuade Robert that saying that a [work package](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e240) could follow a [procedure](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e134) was not untrue or indeed misleading. An hour later they emerged with [a single new predicate](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e278). But happy.

### Data platform

Following on from [Chris' monster query last week](https://ukparliament.github.io/Weeknotes/2018/50/#employee-of-the-week), Samu made us a [sweet little URL shortener](https://api.parliament.uk/s). So the work of Chris' SPARQL spanner can now be invoked by [api.parliament.uk/s/b89efe80](https://api.parliament.uk/s/b89efe80) and Samu's epic procedure schema visualisation query as [api.parliament.uk/s/e756472e](https://api.parliament.uk/s/e756472e). Like much else, the shortener uses [Pugin](https://github.com/ukparliament/parliament.uk-pugin), the marvellous beta front end courtesy of [Usman](https://twitter.com/_usmanafzal).

Whilst releasing the URL shortener, Samu took the opportunity to update the search service to also use Pugin. Which is [here for your delectation](https://api.parliament.uk/search/query?q=accessible+search).

On the subject of search, more things on the service are now nicely addressable since our Samu added [HTTP accept header](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Accept) - and extension - based [content negotiation](https://en.wikipedia.org/wiki/Content_negotiation) for search results. Which means you can now get back  [JSON](https://api.parliament.uk/search/query.json?q=%22content+negotiation%22), [Atom](https://api.parliament.uk/search/query.atom?q=%22content+negotiation%22), [RSS](https://api.parliament.uk/search/query.rss?q=%22content+negotiation%22) and [good old HTML](https://api.parliament.uk/search/query.html?q=%22content+negotiation%22). Beautiful. Properly nice.

The [OpenSearch document](https://api.parliament.uk/search/description) reflects these options and adds some additional metadata for good luck. As does the [OpenApi document](https://swagger.io/docs/specification/about/), which [is itself content negotiable](https://api.parliament.uk/search/openapi) for lovers of [YAML](https://api.parliament.uk/search/openapi.yaml) or [JSON](https://api.parliament.uk/search/openapi.json). There's even a [public UI for interacting with the service](https://api.parliament.uk/search/) which uses the OpenApi definition. Open your browser. Have a tinker.

Samu would like to add that none of this work required any changes to the website because both the data platform and the website use open standards to exchange search requests and responses. The OpenSearch standard has a [service description mechanism](https://github.com/dewitt/opensearch/blob/master/opensearch-1-1-draft-6.md#opensearch-description-documen), allowing the API publisher - team:Samu - to tell consumers - team:Jamie - how it all works and what to expect. The work here is merely to embrace the standard. Past that point changes become trivial. Which is why we love open standards. Filthy for them, some might say.

On a final search related note, Alex departed last week, but not before gifting us a set of improved search hints which are now live. Date hints also went live round about the same time. His changes can be found at [api.parliament.uk/s/37b8dde7](https://api.parliament.uk/s/37b8dde7) because Samu's URL shortener also works for [github/ukparliament](https://github.com/ukparliament). Obviously. No [amateurs](https://www.youtube.com/watch?v=7wK9on_AL-k) here.

### On topics. And taggings

Team:Samu have also been busy building a [vocabulary browser](https://api.parliament.uk/vocabulary/browser) for use by the Indexing and Data Management Section of the House of Commons Library. And beyond. It's been another collaborative effort with our Matthieu working closely with [librarian Liz](https://twitter.com/greensideknits).

IDMS do sterling work subject indexing parliamentary material and tying together disjointed data. But to date the output of that work has only been half visible behind a [search form](http://search-material.parliament.uk/). And not visible to the wider web. We also [published the thesauri on data.parliament](http://www.data.parliament.uk/dataset/thesauri), but given that was just a list of subject heading and carried no indexed content, it was less that useful.

The new browser spans across the data platform triple store and [SOLR](http://lucene.apache.org/solr/) - where the subject indexings live - so you can now browse parliamentary material by subject heading in a way that's never been possible before. For those interested in approaching Parliament by topic, rather than by business or document type, it's probably a better bet the website.

The vocabulary browser is based on a lot of thinking and a lot of work over a lot of time. Matthieu has been beavering away on exporting our existing vocabulary, converting it to [SKOS](https://www.w3.org/TR/skos-primer/), importing it into a triple store and making the whole thing queryable by SPARQL. We think it's not too off being able to replace [search material](http://search-material.parliament.uk/) and in time could replace the internal only parliamentary search. And it could totally provide the backbone for topic pages on beta. Take a look at what's been [subject indexed under Brexit and we think you'll get our drift](https://api.parliament.uk/s/87ba085c).

It's built on our standard technology stack and makes use of:

* GraphDB, a standard compliant graph database engine supporting [OWL inferencing](https://www.w3.org/standards/semanticweb/inference) and [SPARQL querying](https://www.w3.org/TR/sparql11-query/).

* A standard ontology  for expressing the basic structure and content of concept schemes such as thesauri, classification schemes, taxonomies and other similar types of controlled vocabulary in the shape of SKOS.

* Samu's Dynamic graph implementation which he contributed as an extension to the [dotNet RDF library](https://github.com/langsamu/dotNetRDF.Dynamic).

* A standard, containerised .NET Core web application with fully automated deployment.

* Another outing for Usman's Pugin framework.

* A simple [Lucene](http://lucene.apache.org/) connector for search.

It's another clarion call for the benefits of having a team dedicated to working in the open and working with open standards. And long may that continue. As the Lego bricks get deployed, building standards compliant, accessible applications was becoming more and more like intelligently assembling strong blocks of technology. And every new project benefited from updates on our stack.

Liz and Matthieu gave a brief tour to librarian Phil and his team who were pleased to see the vocabulary available in an accessible and good looking UI. And the adoption of SKOS seems like a good thing to everyone with a bit of subject matter expertise in knowledge management.

It's also lending a helpful hand with improving our vocabulary, as Matthieu and Liz collaborate on tidying and pruning the hierarchy.

Every week, more brilliant work when librarians met team:Samu.

### Were new facts uncovered?

We could tell you. But we'd have to shoot you.

### What we're listening to

This week we've been mostly listening to [Insight](https://www.youtube.com/watch?v=iXt6CNKqLVQ). It seems to match our current festive mood.