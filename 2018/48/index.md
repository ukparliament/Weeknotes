## 2018 Week 48

### Man flu

For the last couple of weeks, your regular correspondent has been struck down with a terrible dose of man flu. Which means he’s been slightly outside of the loop. Not a clue what’s going on. So this edition may be lacking in both coverage and detail. We can only ever do our best.

### Community

Team:[Samu](https://twitter.com/langsamu) were joined by [Connel McKeown](https://pure.qub.ac.uk/portal/en/persons/connel-mckeown(d834a936-cb6e-4c84-ba7a-6a1f17714cf9).html), a PhD student at [Queen's University Belfast](https://www.qub.ac.uk/) who's writing his dissertation on "the implications of open data for government accountability". He [got in touch](https://twitter.com/ConnelMckeown/status/1044197277143904257) a while back to see if he could drop by for a chat. And last Friday he boarded a plane for London to interview [Chris](https://twitter.com/chrisalcockdev), [Anya](https://twitter.com/bitten_), [Jamie](https://twitter.com/oddtype) and Robert, and spend some time talking to the rest of the team. Luckily for Connel, his visit coincided with Private Members’ Bill day. He managed to catch a glimpse of the [Commons Chamber debate on the Parking (Code of Practice) Bill](https://hansard.parliament.uk/Commons/2018-11-23/debates/005F9F65-57E5-4AD0-B6EC-C26C75A7AAA2/Parking(CodeOfPractice)Bill). We hope he found the conversations and the debate both riveting and useful.

A couple of weeks back we reported that the [ODI](https://theodi.org/)'s [Leigh Dodds](https://twitter.com/ldodds) had completed his report on how we might model statistics in the data platform, recommending we bin our [stats-series model](https://ukparliament.github.io/ontologies/stats-series/stats-series-ontology.html) and instead use [RDF data cube](https://www.w3.org/TR/vocab-data-cube/). Leigh has since given us permission to publish the report, it’s [here on GitHub](https://github.com/ukparliament/Weeknotes/blob/master/external-reports/odi/statistical-data/recommendations.pdf) together with a [zip file of examples](https://github.com/ukparliament/Weeknotes/blob/master/external-reports/odi/statistical-data/data-cube-examples.zip). Hopefully it might be of use to other people.

Chris continued our fruitful collaboration with the [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) community via the medium of [Andrew Gray](https://twitter.com/generalising). As of this week, we're linking around 2000 of our [Members](https://api.parliament.uk/query/resource?uri=https://id.parliament.uk/schema/Member) to their equivalent Wikidata URI. Chris has sent a spreadsheet of the mappings to Andrew. Wikidata have an [open proposal for a UK Parliament  identifier property](https://www.wikidata.org/wiki/Wikidata:Property_proposal/UK_Parliament_Identifier) which we're hoping Andrew will be able to start populating once the property is ratified.

### One world, one web, one team

A couple of weeks back House of Commons [Jack](https://twitter.com/jackpdent) sent us some short descriptions he'd written for the procedures we've modelled so far. Anya, Robert and [Michael](https://twitter.com/fantasticlife) had promised to review and edit but their best intentions were laid waste by the man flu outbreak. On Friday afternoon they finally sat down in Michael's office where Robert took out his scalpel and started chopping. The [finely sculpted results](https://ukparliament.github.io/ontologies/procedure/procedure-descriptions/) are in GitHub.

### Domain modelling

Anya and Robert left the library to visit Samu and Chris for further conversations around adding logic gates to the [procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html). A saga that's been rumbling on for some weeks. They presented Michael's new option of removing logic gates as a separate thing and instead treating them as a special type of step. Which everyone seemed happy with. Samu has always been keen to replace all of the [route typing](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e395) with logic gates. Michael was less convinced. But Samu won, as we always knew he would. The new proposal involves treating all routes as causes, using a NOT gate to describe precludes and using a new choice or option or decision step to describe allows. The latter bit being Chris's brainwave. The published model is now a little out of date and needs a serious prune. But that can wait for next week. In the meantime, Chris is experimenting with migrating some of the current data to its new shape. We wait and hope.

Anya and Michael attempted to triage various bits and bobs of documentation around procedural data. We currently have the [flowcharts](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#flowcharts) which label [steps](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e408) in one way, the instance data that labels them in another way, and a spreadsheet that maps between the two. Michael made a start on editing the flowcharts, updating the step labels and reshaping the House bubbles. So far he's tinkered with the [draft negative procedure](https://ukparliament.github.io/ontologies/procedure/flowcharts/sis/draft-negative.pdf), the [draft affirmative procedure](https://ukparliament.github.io/ontologies/procedure/flowcharts/sis/draft-affirmative.pdf) and the [proposed negative statutory instrument procedure](https://ukparliament.github.io/ontologies/procedure/flowcharts/proposed-negative-sis/proposed-negative-sis.pdf). The last two still need a second eye. Elsewhere Anya checked the spreadsheet aligned with the instance data. Chris helped out with a handy [SPARQL](https://en.wikipedia.org/wiki/SPARQL) query to list out current step names and Houses. Lots of changes were made. Peace and harmony reigned. Until we found that the changes had gone missing on their way to the mythical cloud. Because SharePoint syncing is shit. Utter shit.

On Friday morning, Anya, Robert and Michael were happily reunited with House of Lords Jane and House of Commons Jack to dive once more into the parliamentary procedure for treaties. Whiteboards were filled, the [Constitutional Reform and Governance Act 2010](https://www.legislation.gov.uk/ukpga/2010/25/contents) was consulted, heads were scratched and shoulders shrugged. And, there weren’t too many changes from last time. They stripped out deferred divisions in the Commons, added the possibility of Lords debates in Grand Committee, and deleted assorted arrows as realisation dawned that the Lords has even less say in any of this than they once thought. The [new flowchart is in the usual GitHub repo](https://github.com/ukparliament/ontologies/blob/master/procedure/flowcharts/logic/treaties.pdf). They're working on the assumption that it's not finished because nothing is ever finished. The step labels need a little more attention. but for now they think they’ve taken it about as far as they can.

### Data platfrom

Wojciech has made a couple of changes to the procedure editor. The first one is fairly minor, allowing us to associate a slug of descriptive text with a procedure. The second one could have more profound implications for the way we manage procedural data. The current model allows a [route](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e382) to belong to one and only one procedure. But some routes are common across multiple procedures. The working example is the bunch of routes connecting various steps around English Votes for English Laws (EVEL) certification, all of which happen in all four SI procedures. Wojciech’s second change to the procedure editor allows routes to belong to more than one procedure, which means we can identify procedures within procedures, such as EVEL certification.



Over time we want to identify mini-procedures like EVEL certification and make them one bunch of routes in multiple procedures. This opens up the possibility of not only minimising the number of routes we need but also making procedures more granular and more modular. Which would be super.

### Strolls

Not bloody likely. Atchoo.

### Things that caught our eye

* [Who’s Working for Your Vote?](https://ourdataourselves.tacticaltech.org/posts/whos-working-for-vote/). An investigation into how personal data is used in political campaigns.

* [Open Access UK](https://openaccess.transparency.org.uk/). Who's meeting government, when and for what purpose.

### What we're listening to

Anya and Robert took off to the wilds of north London to witness the legend that is [Idris Ackamoor](https://en.wikipedia.org/wiki/Idris_Ackamoor). And his Pyramids. The great man was spotted sauntering through the crowds covered in lamé and bearing what looked to be a didgeridoo. Splendid stuff we're told.

Michael meanwhile has been finding it hard to escape the [Wet Nuns](https://en-gb.facebook.com/wetnuns/). His sickbed echoed to the marvellous sound of [Throttle](https://www.youtube.com/watch?v=bcqk0tEwGjw). He could listen but not look.

