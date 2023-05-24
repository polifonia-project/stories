---
component-id: William#1_EuropeanFolkMusic
name:  "European Folk Music" 
type: Story
description: "William is looking for songs matching his search criteria from the 20th and 21st centuries, across various music collections in Europe (particularly folk music)."
related-components:
  - persona:
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
story type:
  - expert driven
---

# European Folk Music

## Persona
William is an art historian working as a curator for the Europeana platform. As such he’s aiming to reach a large audience with transnational heritage stories to educate and inspire European citizens. He lacks in-depth musicological knowledge.

## Goal
William wants to create online exhibitions that illustrates themes such as:
- the interconnectedness of (folk) songs of the early 20th century across Europe.
- the connections between prominent 20th and 21st century European composers.

## Scenario
William is looking for songs matching his search criteria from the 20th and 21st centuries, across various music collections in Europe (particularly folk music). He is interested in descriptions of the songs, descriptionsn of performances/recordings, sheet music, and actual audio(visual) content. He wants to see patterns in the metadata of these songs, such as developments over time, location or over genres, that can give him clues about connections and influences. He also wants to be able to find interesting connections between composers, compositions and performers across the boundaries of the various archive(s) they are listed in. William wants to use such patterns and connections to provide an overview of the cultural/musical interchange between various European Countries pre- and post-WWII. 

At present, William must do a lot of laborious manual work, consulting different search portals separately and then attempting to integrate the results himself in documents and spreadsheets. He must often look people up in different sources to find out more about them, to give context to the results he finds. He has to cope with different naming conventions and typos in the labels used for compositions, composers and performers in the separate archives, spending a lot of time thinking up possible variations on his search terms. In addition, for each new archive he needs to go in search of documentation that will explain the meaning of the metadata fields and their completeness, often needing to email and ring up the archive owners to find out who has the information he needs. Otherwise he may fail to formulate his query correctly, or misinterpret his search results.

Thanks to Polifonia, William will be presented with one set of integrated results for songs from across the archives. His results will be enriched with additional information about the persons and compositions found, and accompanied by useful links to related persons and compositions. These links will be visualised in a way that helps him to understand the connections between persons and compositions. Distributions of his set of search results over time, location, and other aspects such as genre will be visualised so that he can spot patterns. He will have easy access to information about the metadata of the collections and statistics on its completeness. 

## Example data

### Cataloguing information
- Thesauri of composers and performers, (and to a lesser extent events, subjects and locations) represented in ontologies shared by multiple collections. These entities can be used to consistently find archival records with annotations connected to the respective composers and performers of interest. An example of a shared vocabulary in use at NISV and other Dutch cultural heritage organisations is the '[Common Thesaurus Audiovisual Archives (GTAA)](http://labs.beeldengeluid.nl/datasets/gtaa)', containing term categories such as Person names, Classification, Genre, Geographical Names, Names and Subjects. Vocabularies typically contain a label and alternative labels, but may also have additional information such as occupation of a person, or the hierarchy between subjects. An example of a composer represented in the GTAA: https://data.beeldengeluid.nl/gtaa/77493
- Wikidata entities for compositions, composers and performers (and to a lesser extent events, subjects and locations). This data can help to augment collection records with additional information, including biographical information, images and links to significant works and other persons. It can also assist in linking thesauri or expanding search queries with alternative labels to compensate for variations in naming conventions and typos. An example of a Wikidata entity for a composer: https://www.wikidata.org/wiki/Q504743
- Entries in other databases for compositions, composers and performers. E.g. Discogs. As for Wikidata, this data can help with augmenting records with additional information and linking across archives. An example of a composer in Discogs: https://www.discogs.com/artist/171391-Louis-Andriessen
- Audiovisual archival records (e.g. LPs, concert recordings, TV and Radio programmes) with annotations connecting them to the respective composers and performers of interest. They also contain information about time, location and other aspects such as genre. This information can be aggregated to spot patterns in sets of results and compare them in different collections, e.g. a performer who starts on the radio, appears with increasing frequency and then moves to television. Alternative titles and related titles (e.g. album and track titles) can help in disambiguating and correctly identifying compositions. These records can be accessed e.g. as [Schema.org](https://schema.org/) based Linked Data via a SPARQL endpoint. See for example [this query](https://cat.apis.beeldengeluid.nl/sparql#transientDatasources=https%3A%2F%2Fcat.apis.beeldengeluid.nl%2Fsparql&query=PREFIX%20rdf%3A%20%3Chttp%3A%2F%2Fwww.w3.org%2F1999%2F02%2F22-rdf-syntax-ns%23%3E%0APREFIX%20rdfs%3A%20%3Chttp%3A%2F%2Fwww.w3.org%2F2000%2F01%2Frdf-schema%23%3E%0APREFIX%20sdo%3A%20%3Chttps%3A%2F%2Fschema.org%2F%3E%0APREFIX%20skos%3A%20%3Chttp%3A%2F%2Fwww.w3.org%2F2004%2F02%2Fskos%2Fcore%23%3E%0A%0ASELECT%20DISTINCT%20%3FprogramId%20%3Fmain_title%20%3Fgtaa_concept%20%3Fperson_name_pref_label%20%0AWHERE%20%7B%0A%20%20VALUES%20%3Fperson_name_pref_label%20%7B%0A%20%20%20%20'Andriessen%2C%20Louis'%0A%20%20%7D%0A%20%20%0A%20%20%3FprogramId%20a%20sdo%3ACreativeWork%20.%20%0A%0A%20%20%3FprogramId%20(sdo%3Aabout%7Csdo%3Amentions%7Csdo%3Acreator%7Csdo%3Acontributor%7Csdo%3Aactor%7Csdo%3Acrew%7Csdo%3Aperformer)%2F%0A%20%20(sdo%3Aabout%7Csdo%3Amentions%7Csdo%3Acreator%7Csdo%3Acontributor%7Csdo%3Aactor%7Csdo%3Acrew%7Csdo%3Aperformer)%20%3Fgtaa_concept%20.%0A%0A%20%20%3Fgtaa_concept%20skos%3AprefLabel%20%3Fperson_name_pref_label.%0A%20%20%3FprogramId%20sdo%3Aname%20%3Fname%20.%0A%0A%20%20BIND(str(%3Fname)%20as%20%3Fmain_title)%0A%7D%20LIMIT%2020) for collection items related to the composer Louis Andriessen.
- Description of collection metadata. For example [this collection description](https://mediasuitedata.clariah.nl/dataset/audiovisual-collection-daan) contains [a list of metadata fields and their descriptions](https://mediasuitedata.clariah.nl/dataset/7879cf23-3ac7-4f27-9b3a-475b0c3b499f/resource/9f9bdb43-4be6-4019-b845-8b14f884745f/download/fielddescriptions.tsv), 


## Competency questions
CQ1: In which collections/datasets does song X occur?

CQ2: In which countries does song X occur?

CQ3: Which compositions match with William's thematic focus for the exhibition?

CQ4: Which composers and performers are related to these compositions?'

CQ5: In which historical documents is composer X mentioned?

CQ6: Under which titles is this song known? (multi-language)

CQ7: What are the relations between the relevant countries, compositions, composers and performers in the various collections?

CQ8: How have the relations between the relevant countries, compositions, composers and performers in the various collections changed over time?

CQ9: How many search results are there per time period?

CQ10: How many search results are there per genre?

CQ11: What is the relevant metadata for music collections and what do the different fields mean?

CQ12: Inspect the degree to which metadata fields have been filled across the collections, see trends and gaps?
