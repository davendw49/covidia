# covidia

<div style="text-align:center">
<img src="https://big-cheng.com/covidia/logo.png" alt="covidia-logo" width="600"/>
<h2>C🦠vidia: COVID-19 Interdisciplinary Academic Knowledge Graph</h2>
</div>


The SPARQL Endpoint is **[https://covidia.acemap.info/sparql](https://covidia.acemap.info/sparql)**

## Overview

Covidia is an Interdisciplinary Academic Knowledge Graph for COVID-19 by fusing papers' illustrations, text, inner knowledge and bibliometric data. To our knowledge, Covidia is currently the first interdisciplinary academic knowledge graph during the pandemic. Figure 1 shows the schema of the Covidia. And if you want to explore the Covidia data, try [https://snorql.acemap.cn/Covidia](https://snorql.acemap.cn/Covidia).

<div style="text-align:center">
<img src="https://big-cheng.com/covidia/overview.png" alt="covidia-logo" width="800"/>
<h6>Figure 1. Schema graph of the COVID-19 Interdisciplinary Academic Knowledge Graph (Covidia) </h6>
</div>

And schemagraph file stored in N-Triple form and the ontology file including concept's data properties and object properties stored in pair can be downloaded from:

|schemagraph|ontologies|
|:-:|:-:|
|[schema]	|[ontology]|

Also, the developers can use the PREFIX set as follows, the ace/covid/geo is the prefix for concept URI, acer/covidr is the prefix for object properties and covidp/acep belongs to data properties.

- PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#\>
- PREFIX rdfs: <http://www.w3.org/2000/01/rdf-schema#\>
- PREFIX foaf: <http://xmlns.com/foaf/0.1/\>
- PREFIX skos: <http://www.w3.org/2004/02/skos/core#\>
- PREFIX acep: <https://www.acekg.cn/property/\>
- PREFIX acer: <https://www.acekg.cn/relation/\>
- PREFIX ace: <https://www.acekg.cn/concept/\>
- PREFIX geo: <https://www.acekg.cn/concept/geo/\>
- PREFIX covidiap: <https://covidia.acemap.info/property/\>
- PREFIX covidiar: <https://covidia.acemap.info/relation/\>
- PREFIX covidia: <https://covidia.acemap.info/concept/\>
- PREFIX owl: <http://www.w3.org/2002/07/owl#\>


## Downloads

The download links are as follows: (the values in parentheses are the number of all the COVID-19-
related papers during the pandemic)

| **Concept** | **Link**              |    **Count**        |    | **Concept**      | **Link**              |  **Count**        |
|-------------|-----------------------|---------------------|----|------------------|-----------------------|-------------------|
|paper        | [covidia:paper]       | 231,293 (1,107,008) |    | topic            | [covidia:topic]       | 15,289 (17,334)   |
|author       | [covidia:author]      | 928,932 (2,599,342) |    | discipline       | [covidia:discipline]  | 22 (22)           |
|organization | [covidia:institute]   | 16,078 (28,266)     |    | papertable       | [ace:papertable]      | 129,873 (543,418) |
|journal      | [covidia:journal]     | 12,339 (18,656)     |    | illustration     | [ace:illustration]    | 232,953 (817,539) |
|conference   | [covidia:conference]  | 25,288 (38,192)     |    | knowledge        | [covidia:knowledge]   | 563,932 (794,187) |
|preprint     | [covidia:preprint]    | 62 (62)             |    | location         | [geo:location]        | 21,349 (38,465)   |
|venue        | [covidia:venue]       | 37,689 (56,910)     |    | geohash          |                       | 21,349 (38,465)   |
|**Total**    |                       |                     |    |                  |                     |2,366,321 (6,097,866)|

| **Relation**     | **Link**                                              |    **Count**         |    | **Relation**     | **Link**               |  **Count**            |
|------------------|-------------------------------------------------------|----------------------|----|------------------|------------------------|-----------------------|
|is_cited_by       | [covidr:is_cited_by-covid],[covidr:is_cited_by-acemap]| 982,381 (4,791,970)  |    | work_in          | [covidr:work_in]       | 412,983 (1,370,233)   |
|is_written_by     | [covidr:is_written_by]                                | 1,823,286 (5,320,076)|    | is_located_in    | [covidr:is_located_in] | 56,212 (14,158)       |
|is_published_in   | [covidr:is_published_in]                              | 301,064 (803,880)    |    | has_papertable   | [acer:has_papertable]  | 129,873 (543,418)     |
|in_the_topic_of   | [covidr:is_about]                                     | 619,529 (1,945,205)  |    | has_illustration | [acer:has_illustration]| 232,953 (817,539)     |
|belongs_to        | [covidr:belongs_to_1]                                 | 482,297 (2,451,189)  |    | paperkg_relation |                        | 1,029,834 (3,829,201) |
|mention_knowledge | [covidr:mention_knowledge]                            | 306,829 (1,228,392)  |    | rdfs:subClassOf  |                        | 11,086 (45,231)       |
|mention_location  | [covidr:mention_location]                             | 197,235 (750,738)    |    | owl:sameAs       | [owl:sameAs(cite)]     | 563,932 (794,187)     |
|**Total**         |                                                       |                      |    |                  |                        |7,149,494 (24,705,417))|
 
## Pipeline on Glossary and linking to the COVID-19 papers

All the supplements can be downloaded from [Google Drive](https://drive.google.com/drive/folders/1KyDLxjGEpFttM1mtg3F2CiogqF5kOAbl?usp=sharing)

### Glossary and Discipline KGs

- Glossary

| **id** 	|                 **Disciplines**                	|                  **Glossary**                  	|                                  **URL**                                  	|
|:------:	|:----------------------------------------------:	|:----------------------------------------------:	|:-------------------------------------------------------------------------:	|
|  **1** 	|            **Mathematical Sciences**           	|                    mathwords                   	|                    http://www.mathwords.com/a_to_z.htm                    	|
|  **2** 	|              **Physical Sciences**             	|        Glossary_of_physics in Wikipedia        	|             https://en.wikipedia.org/wiki/Glossary_of_physics             	|
|  **3** 	|              **Chemical Sciences**             	|    Glossary of chemistry terms in Wikipedia    	|         https://en.wikipedia.org/wiki/Glossary_of_chemistry_terms         	|
|  **4** 	|               **Earth Sciences**               	|       Geology and Earth and Science Terms      	|                     http://39.106.163.147/KgEditorWeb/                    	|
|  **5** 	|           **Environmental Sciences**           	| Glossary of environmental science in Wikipedia 	|      https://en.wikipedia.org/wiki/Glossary_of_environmental_science      	|
|  **6** 	|             **Biological Sciences**            	|               biology dictionary               	|         https://biologydictionary.net/complete-list-biology-terms/        	|
|  **7** 	|    **Agricultural and Veterinary Sciences**    	|                                                	|                                                                           	|
|  **8** 	|     **Information and Computing Sciences**     	|            Computer Hope Dictionary            	|                  https://www.computerhope.com/jargon.htm                  	|
|  **9** 	|                 **Engineering**                	|             engineering-dictionary             	|                  https://www.engineering-dictionary.com/                  	|
| **10** 	|                 **Technology**                 	|                                                	|                                                                           	|
| **11** 	|         **Medical and Health Sciences**        	|        Glossary of medicine in Wikipedia       	|             https://en.wikipedia.org/wiki/Glossary_of_medicine            	|
| **12** 	|        **Built Environment and Design**        	|                                                	|                                                                           	|
| **13** 	|                  **Education**                 	|                                                	|                                                                           	|
| **14** 	|                  **Economics**                 	|       Glossary_of_economics in Wikipedia       	|            https://en.wikipedia.org/wiki/Glossary_of_economics            	|
| **15** 	| **Commerce, Management, Tourism and Services** 	|           Glossary of Business Terms           	|          https://www.powerhomebiz.com/glossary-of-business-terms          	|
| **16** 	|          **Studies in Human Society**          	|                 Sociology Guide                	|                 https://sociologyguide.com/basic-concepts/                	|
| **17** 	|      **Psychology and Cognitive Sciences**     	|  Glossary of Psychology Terms and Definitions  	|     https://psychologenie.com/glossary-of-psychology-terms-definitions    	|
| **18** 	|            **Law and Legal Studies**           	|           Political Science Glossary           	| http://www2.cruzio.com/~zdino/psychology/political.science.glossary.htm#a 	|
| **19** 	|    **Studies in Creative Arts and Writing**    	|      The Art History Archive - Terminology     	|           http://www.arthistoryarchive.com/arthistory/glossary/           	|
| **20** 	|     **Language, Communication and Culture**    	|           Materials Science Glossary           	|         https://www.dierk-raabe.com/glossary-of-materials-science/        	|
| **21** 	|           **History and Archaeology**          	|        Emerson's wee history dictionary        	|             http://www.emersonkent.com/history_dictionary.htm             	|
| **22** 	|      **Philosophy and Religious Studies**      	|  A Dictionary of Philosophical Terms and Names 	|                     http://www.philosophypages.com/dy/                    	|

## Citation

We now have a [paper](#) under review on CIKM Applied Research Track:
```bibtex
@inproceedings{covidia,
    title = "Covidia: COVID-19 Interdisciplinary Academic Knowledge Graph Construction and Application",
    author = "Cheng Deng, Zhang Tianhang, Bo Tong, Yuting Jia, Luoyi Fu, Jiaxin Ding, Weinan Zhang, Xinbing Wang and Chenghu Zhou",
}
```

[schema]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/schema.nt
[ontology]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/ontology.nt

[covidia:paper]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_paper.nt
[covidia:author]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_author.nt
[covidia:institute]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_institute.nt
[covidia:venue]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_venue.nt
[covidia:journal]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_venue.nt
[covidia:preprint]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_venue.nt
[covidia:conference]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_venue.nt

[covidia:topic]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_topic.nt
[covidia:knowledge]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_knowledge.nt
[covidia:discipline]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_discipline.nt
[ace:illustration]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_illustration.nt
[ace:papertable]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_papertable.nt
[geo:location]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/cakg-concept_location.nt

[covidr:is_cited_by-covid]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_is_cited_by_covid.nt
[covidr:is_cited_by-acemap]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_is_cited_by_am.nt
[covidr:is_written_by]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_is_written_by.nt
[covidr:work_in]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_work_in.nt
[covidr:is_about]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_is_about.nt
[covidr:mention_location]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_mention_location.nt
[covidr:belongs_to_1]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_belongs_to_glossary.nt
[covidr:is_published_in]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_is_published_in.nt
[acer:has_illustration]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_has_illustration.nt
[acer:has_papertable]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_has_papertable.nt
[covidr:mention_knowledge]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_mention_knowledge.nt
[covidr:is_located_in]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_is_located_in.nt
[geo:has_geohash]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/rel_has_geohash.nt
[owl:sameAs(cite)]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/sameas_cite.nt
