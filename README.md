# tate-skos
This repository features a [SKOS](https://www.w3.org/2004/02/skos/) taxonomy generated from Tate's subject hierarchy through the use of Catalink's proprietary semantic data integration framework [CASPAR](https://caspar.catalink.eu/). 


## Scope & Aim
[Tate UK](https://www.tate.org.uk/) has publicly released its subject hierarchy as a [set of JSON files](https://github.com/tategallery/collection/tree/master/processed/subjects) organized in three levels. For example, in [this artwork](http://www.tate.org.uk/art/artworks/blake-a-figure-bowing-before-a-seated-old-man-with-his-arm-outstretched-in-benediction-a00001) by Robert Blake, the relevant subjects are found in section 'Explore'. An excerpt from the specific subjects is `'religion and belief' > 'universal religious imagery' > 'blessing'`. The following table indicates the total number of subjects per level:

|  Level  | Count |
|:-------:|:-----:|
| level-0 |   16  |
| level-1 |  142  |
| level-2 |  2251 |

The aim of this work was to assess how easy it is to deploy our [CASPAR framework](https://caspar.catalink.eu/) for converting the set of JSON files into a SKOS taxonomy. Having the subject hierarchy in SKOS format enables its easy publication and use by third parties as [linked data](https://en.wikipedia.org/wiki/Linked_data).


## Semantic Data Integration with CASPAR
CASPAR converts the input files into a semantic [Knowledge Graph](https://en.wikipedia.org/wiki/Knowledge_graph) (KG) - in this case, an RDF SKOS taxonomy - through the definition of mappings between input data fields and respective ontology concepts. The specification of mappings is compliant with a proprietary Domain-Specific Language (DSL) based on JSON syntax.

Just for reference, the mappings for converting Tate's JSON files into a SKOS taxonomy via CASPAR are found [here](resources/mappings).


## SKOS taxonomy
The resulting SKOS taxonomy can be found [here](). Through [SKOS Play](https://skos-play.sparna.fr/play/) we also generated the subject tree (see figure below), as well as the [complete documentation](resources/documentation/tate-skos-documentation.pdf) in PDF, containing the alphabetical index of the subjects with attributes on each entry (notation, broader, narrower, related, all notes), followed by a clickable hierarchical tree that directs to entries in the alphabetical index.

![tate-skos-play.png](resources/figures/tate-skos-play.png)


## Contact Details
For any queries or remarks on the Tate SKOS taxonomy, or if you would like to deploy CASPAR for your use case, please feel free to [contact us](mailto:caspar@catalink.eu?subject=Tate%20SKOS).