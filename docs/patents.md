# Dan McCrary's Patents

## Links
[Justia Patents](https://patents.justia.com/inventor/daniel-g-mccreary)

## Patents Granted

### Semantic Search
* [Automated concepts for interrogating a document storage database](https://patents.google.com/patent/US11204950B2/en) - this is the
technology that many people call "semantic search" today.  I really
didn't think this was that novel.  It seemed like just common sense.

I think that if Optum wanted to, they could generate substantial defending this patent since today many people use the process I outlined in the patent.
Today many companies use semantic search in many products.  They should all be grateful that Optum is not trying to turn this patent into a revenue generator.

## Patents Pending

### Predictive Recommendation for Schema Mapping

Inspired by the 1970 science fiction movie [Collossus: The Forbin Project](https://en.wikipedia.org/wiki/Colossus:_The_Forbin_Project), I have spent many hours pondering
how I could automatically make two computers talk to each other.  The secret is matching metadata, and it is the inspiration for this important patent.

**Publication number:** 20230229639<br/>
**Type:** Application<br/>
**Filed:** Jan 18, 2022<br/>
**Publication Date:** Jul 20, 2023<br/>
**Inventors:** Daniel G. McCREARY (St. Louis Park, MN), Joshua A. MEEKHOF (Grand Rapids, MI)<br/>
**Application Number:** 17/577,807<br/>
**US Patent Application Number:** #20230229639<br/>
**International Classification:** G06F 16/21 (20060101); G06N 20/00 (20060101);

This patent covers the process of using both deterministic rules and embeddings to suggest mappings between a new dataset schema and an existing canonical schema.  Today, anyone building a data warehouse on complex data knows how difficult and time consuming this task is.  This patent covers a process that I have been working on for over ten years, far before I joined Optum.

The process involves building a JSON document for each data element in both a canonical internal schema and for new data being loaded into that schema.  Each JSON file includes metadata about that data element including names, data types, definitions, and data profiles.

There are four factors in matching data elements:

1. **Lexical Information** such a the name of the data element or it's alias
2. **Linguitic Informatin** such as the definition or how it is ued
3. **Semantic Inforamtion** such as a URI to a data dictionary that defines this data element
4. **Data Profile** such as the data type, enumerated values, statistical distribution including time-of-day, day-of-week or other temporal pattern matches.

Each of factors are converted into documents or document fragments and embedding are created to be used to compare each new incoming data element with existing canonical schema elements.
Weighting rules are also applied.  For example an exact match of a URI to a certified data registry overrides all other rules.

When I first stated building these systems with [Josh Meekhof](https://www.linkedin.com/in/joshua-meekhof/) we were only getting about a 70% match rate on our target of 500 data element schemas.  However, since then, LLMs have created embeddings for things like data element definitions that allow the match rate to rise to over 90%.  I continue to work with my friend [Loren Cahlander](https://www.linkedin.com/in/lorencahlander/) to promote high-quality user interfaces to these tools.  Loren's code base still runs on the ultra-cool eXist-DB system and is written in XQuery.

* [Link on Justia Patents](https://patents.justia.com/patent/20230229639)

* [PREDICTIVE RECOMMENDATIONS FOR SCHEMA MAPPING](https://github.com/dmccreary/dmccreary/blob/master/docs/patents/Predictive-Schema-Mapper.pdf)

* [PREDICTIVE RECOMMENDATIONS FOR SCHEMA MAPPING Figures](https://github.com/dmccreary/dmccreary/blob/master/docs/patents/Predictive-Schema-Mapper-Figures.pdf)

### Clinical Cohorts
* [Machine learning techniques for generating cohorts and predictive modeling based thereof](https://patents.google.com/patent/US20240047070A1) - with [Mark Megerian](https://www.linkedin.com/in/mark-megerian-7aa08984/)]

### Genetic Risk Scores
* [Machine learning techniques for generating hybrid risk scores](https://patents.google.com/patent/US20220122736A1/en)

### Recalculation of Risk Scores
* [Machine learning techniques for generating recalculation determinations for predicted risk scores](https://patents.google.com/patent/US20220327404A1/en?q=(Daniel+George+McCreary))

## Ontology Change Graph Publishing
* [Justia Patents](https://patents.justia.com/patent/20230342587)
* [ONTOLOGY CHANGE GRAPH PUBLISHING SYSTEM](https://trea.com/information/ontology-change-graph-publishing-system/patentapplication/a298416e-c85d-4959-9ca9-5ea875069a8e) with [Jeff Winkler]




