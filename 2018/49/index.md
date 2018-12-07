## 2018 Week 49

### Man flu (slight return)

After what seemed like recovery, man flu returned with a vengeance and another day in bed beckoned for your regular correspondent. Although, this may not have been helped by beer. [Michael](https://twitter.com/fantasticlife) is thankfully [fit and working again](https://www.youtube.com/watch?v=QnxZkK4mdM8). At least until the next pub exerts its charms. Never drink with librarians is a lesson he finds hard to learn.

### Community

[Our Dan](https://twitter.com/dasbarrett) finally fulfilled his dream of an overseas business trip. [Here he is](https://twitter.com/dasbarrett/status/1069529380366548993) at the [Inter-Parliamentary Union](https://twitter.com/IPUparliament) e-Parliament conference. See how smart he looks in his tie and his jacket and his gansey. His mam must be well proud.

[Chris](https://twitter.com/chrisalcockdev) and [Andrew](https://twitter.com/generalising) pulled off a one web win. As of this week, we not only have links to Wikidata from our data platform, Wikidata now has a [property to link to us](https://www.wikidata.org/wiki/Property:P6213). Unlike the old biography page property, P6213 can identify anything in the data platform from Members to constituencies to parties to [parliament periods](https://ukparliament.github.io/ontologies/time-period/time-period-ontology.html#d4e487) to committees to procedures. Anything and everything really. P6213, you are native to a web of data and we love you.

### One world, one web, one team

[Anya](https://twitter.com/bitten_), Robert and Michael met with [James](https://twitter.com/TheVinternets) and Simon from the committee website "product" team. They chatted about domain models and the expression thereof. Michael made his usual point that beauty lives in bone structure. And not in the over rigorous application of Max Factor lippy. Let the bones of the model show through in the view. As a [great man](https://en.wikipedia.org/wiki/Eric_J._Evans) once said.

James drifted back to Tothill Street, this time in the company of House of Commons James and House of Lords Ed. They met with Anya, Robert and Michael to chat about the URIs we'll need to slice and dice committees by House, type, scrutiny area and currency. They think they got most of the way there but the conversation got dragged into deeper weeds about URI structure of subclasses and when to make links and when to not make links. Always, said Robert and Michael. You always make links. Or you work on something that isn't the web.

On Wednesday Anya, Robert and Michael left the creature comforts of Michael's office and ventured to the Terrace cafeteira, a popular venue for all kinds of parliamentary mouses. They met House of Commons [Jack](https://twitter.com/jackpdent) to talk about [procedure descriptions](https://ukparliament.github.io/ontologies/procedure/procedure-descriptions/). There remains an open question about what counts as a data attribute - a string literal? - vs what counts as 'content' - a string literal with some markup? Robert talked about [StretchText](https://en.wikipedia.org/wiki/StretchText). Michael argued against making glory holes. Jack asked Michael to please stop saying glory holes. Anya covered her delicate ears. Then Michael fell asleep on the table. Because the man flu was back.

### Domain modelling

With much scalpel wielding from Anya and Robert and some helpful interventions from Jack, Michael finally published some words on [our attempts to teach machines about parliamentary procedure](http://smethur.st/posts/176135869). If you're reading this - hi [Philip](https://twitter.com/PhilDRobertsd) - you might want to take a look at that.

Robert and Michael sat down to redraw and retype the [procedure model](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html). It now features [logic gates](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e309) as a special kind of step and Chris's innovation of [decision steps](https://ukparliament.github.io/ontologies/procedure/procedure-ontology.html#d4e281) to represent allowed but non-causal routes. The comments still need work.

### Data platform

In the course of writing his post, Michael found the [procedure visualisations](https://procedures.azurewebsites.net/Procedures/3/graph) were no longer working. Samu suspected this might have been a side effect of [making routes many-to-many with procedures](https://ukparliament.github.io/Weeknotes/2018/48/#data-platfrom). Wojciech stepped in and fixed things within minutes. Thanks Wojciech.

[Jianhan](https://twitter.com/jianhanzhu) continued in his efforts to investigate the data coming out of the new Committee Information System, in preparation for future orchestration efforts. It's a little like painting your front room by sticking a paint brush through the letterbox. But we do what we can.

[Matthieu](https://twitter.com/cognithive)'s been beavering away to improve our version of [VocBench](http://vocbench.uniroma2.it/) making Java memory management tweaks and working with librarian [Liz](https://twitter.com/greensideknits) on general improvements to the shape of the [vocabulary](http://www.data.parliament.uk/dataset/thesauri). Usman lent a hand so [the whole thing is even starting to look good](https://skosbrowser.azurewebsites.net/schemes).

### Employee of the week....

...goes to employees this week. Congratulations to librarians Jayne and Martin and House of Commons Jack who together thrashed out the question of [parliamentary time travel](https://www.youtube.com/watch?v=PkV0GJ_3NsA). It is generally understood, for some definitions of general and understood, that if a House sits through the night, the date in that House doesn't change until the House rises. It has probably not escaped your attention that the House of Commons has been a little busy this week. On Tuesday they didn't rise until 1:28 am which caused Jayne to question if approval motions passed in the early hours happened on the 4th or the 5th. The question was raised with Jack and triggered some head scratching in the Journal Office. Martin came up with an example from 2000 when the "House sat continuously from 2:30pm on 25th until gone 19:30 on 26th, at all times as far as the House was concerned, it was 25th. Meanwhile in Westminster Hall, the debates scheduled for 26th Jan happened, so [it was 26th Jan in Westminster Hall](https://hansard.parliament.uk/Commons/2000-01-26/debates/229cab3c-29fc-4aa5-be01-de13f7be4c05/SchoolLeagueTables)."

The question of whether an SI being approved in the early hours makes it legislation as of the previous calendar day or the current calendar day was deemed to be, "a matter for the courts." We wonder if [John](https://twitter.com/johnlsheridan) might have a view here?

### Strolls

Not likely. It's impossible to stroll on your back.

### Things that caught our eye

* Anya came across this piece on [being a woman in blockchain](https://breakermag.com/trapped-at-sea-with-cryptos-nouveau-riche/). It's "like riding a bicycle. Except the bicycle is on fire. And everything is on fire. And you are going to hell," we're told. Samu would like to add that this is the major bullshit of our times: AI, blockchain and [quantum computing](https://spectrum.ieee.org/tech-talk/computing/hardware/the-us-national-academies-reports-on-the-prospects-for-quantum-computing). Which reminds him of the other bullshit trinity: product management, user research and service design. He then goes on to compile a trinity of bullshit trinities and includes agile, CD and TDD. He then apologies for his rant.

* Samu spotted this piece on [the friendship that made Google huge](https://www.newyorker.com/magazine/2018/12/10/the-friendship-that-made-google-huge). "To solve problems at scale, paradoxically, you have to know the smallest details. Jeff and Sanjay understood computers at the level of bits."

### What we're listening to

Coughing mainly. Some choking. And rain. Endless rain.