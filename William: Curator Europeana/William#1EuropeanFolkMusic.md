---
id:
- William#1_EuropeanFolkMusic
name:  EuropeanFolkMusic 
persona:
- William
keywords:
- Folk music
- European
- Europeana
- Queries
- Visualisations
work-package:
- WP2
pilot:
- INTERLINK
priority:
- life improver
type:
 - Story
story type:
- expert driven
---

# William#1_EuropeanFolkMusic

## Persona
William is an art historian working as a curator for the Europeana platform. As such he’s aiming to reach a large audience with transnational heritage stories to educate and inspire European citizens. He lacks in-depth musicological knowledge.

## Goal
William wants to create online exhibitions that illustrates themes such as:
- the interconnectedness of folk songs of the early 20th century across Europe.
- the connections between prominent 20th and 21st century European composers.

## Scenario
William is looking for connections between composers, compositions and performers across various collections of 20th century music in Europe, particularly folk music. He wants to be able to find interesting connections between the various archives. William wants to provide an overview of the cultural/musical interchange between various European Countries pre- and post-WWII.

## Example data

- Composers and performers, (and to a lesser extend events, subjects and locations) represented in ontologies shared by multiple collections. These entities can be used to consistently find archival records with annotations connected to the respective composers and performers of interest. An example of a shared vocabulary in use at NISV is the 'Common Thesaurus Audiovisual Archives (GTAA)', containing term categories such as Person names, Classification, Genre, Geographical Names, Names and Subjects. An example of a composer represented in the GTAA: https://data.beeldengeluid.nl/gtaa/77493
- Wikidata entities for composers and performers (and to a lesser extend events, subjects and locations). This data can help to augment collection records with additional information, including images and links to significant works and other persons. An example of Wikidata entity for a composer: https://www.wikidata.org/wiki/Q504743
- Audiovisual archival records (e.g. TV and Radio programmes) with annotations connected to the respective composers and performers of interest, accessed as [Schema.org](https://schema.org/) based Linked Data via a SPARQL endpoint. See for example [this query](https://cat.apis.beeldengeluid.nl/sparql#transientDatasources=https%3A%2F%2Fcat.apis.beeldengeluid.nl%2Fsparql&query=PREFIX%20rdf%3A%20%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0APREFIX%20rdfs%3A%20%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0APREFIX%20sdo%3A%20%3Chttps%3A%2F%2Fschema.org%2F%3E%0APREFIX%20skos%3A%20%3Chttp%3A%2F%2Fwww.w3.org%2F2004%2F02%2Fskos%2Fcore%23%3E%0A%0ASELECT%20DISTINCT%20%3FprogramId%20%3Fmain_title%20%3Fgtaa_concept%20%3Fperson_name_pref_label%20%0AWHERE%20%7B%0A%20%20VALUES%20%3Fperson_name_pref_label%20%7B%0A%20%20%20%20'Andriessen%2C%20Louis'%0A%20%20%7D%0A%20%20%0A%20%20%3FprogramId%20a%20sdo%3ACreativeWork%20.%20%0A%0A%20%20%3FprogramId%20(sdo%3Aabout%7Csdo%3Amentions%7Csdo%3Acreator%7Csdo%3Acontributor%7Csdo%3Aactor%7Csdo%3Acrew%7Csdo%3Aperformer)%2F%0A%20%20(sdo%3Aabout%7Csdo%3Amentions%7Csdo%3Acreator%7Csdo%3Acontributor%7Csdo%3Aactor%7Csdo%3Acrew%7Csdo%3Aperformer)%20%3Fgtaa_concept%20.%0A%0A%20%20%3Fgtaa_concept%20skos%3AprefLabel%20%3Fperson_name_pref_label.%0A%20%20%3FprogramId%20sdo%3Aname%20%3Fname%20.%0A%0A%20%20BIND(str(%3Fname)%20as%20%3Fmain_title)%0A%7D%20LIMIT%2020) for collection items related to the composer Louis Andriessen.

## Competency questions
CQ1: In which collections/datasets does song X occur?

CQ2: In which countries does song X occur?

CQ3: Which compositions match with William's thematic focus for the exhibition?

CQ4: Which composers and performers are related to these compositions?'

CQ5: In which historical documents is composer X mentioned?

CQ6: Under which titles is this song known? (multi-language)

CQ7: Providing a visualisation of relations between the relevant countries, compositions, composers and performers in the various collections and their changes over time

CQ8: Provide overviews of the occurrences of search results across certain time periods or genres.

CQ9: What is the relevant metadata for music collections and what do the different fields mean?

CQ10: Inspect the degree to which metadata fields have been filled across the collections, see trends and gaps?
