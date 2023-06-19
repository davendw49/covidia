# covidia

<p align="center" width="100%">
<img src="https://big-cheng.com/covidia/logo.png" alt="covidia-logo" width="600"/>
<h3 align="center">C🦠vidia: COVID-19 Interdisciplinary Academic Knowledge Graph</h3>
<div align="center" width="100%">
<a href='https://covidia.acemap.info/sparql'><img src='https://img.shields.io/badge/SPARQL%20endpoint-Virtuoso-red'></a> <a href='https://snorql.acemap.cn/Covidia'><img src='https://img.shields.io/badge/SPARQL%20endpoint-SNORQL%20UI-red'></img></a> <a href='https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/'><img src='https://img.shields.io/badge/Dataset-FTP-4169E1'></img></a> <a href='https://drive.google.com/drive/folders/1mWok37-QbLp15daoORekjDANqoek0f3N?usp=share_link'><img src='https://img.shields.io/badge/Dataset-Google%20Drive-4169E1'></img></a> <a href='https://covidia.acemap.info'><img src='https://img.shields.io/badge/Covidia-Platform-F11131'></img></a>
</div>
</p>

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


## Resources Statement

Based on Covidia, we put forward serveral resources, including a COVID-19 interdiciplainary knowledge graph dataset, 4 benchmark collections for network science, natural language processing and data minig, as well as 3 COVID-19-related applications. The detail accessment and statement are listed as follows.

|Resource|URL|Resouce Type|
|:-:|:-:|:-:|
|Covidia Repository|https://github.com/davendw49/covidia|Dataset|
|Covidia Social Network|https://covidia.acemap.info/benchmarks/sn.zip|Benchmark|
|Paper Classification|https://covidia.acemap.info/benchmarks/ipc.zip|Benchmark|
|Knowledge Entity Linking|https://covidia.acemap.info/benchmarks/kel.zip|Benchmark|
|Relation Classification|https://covidia.acemap.info/benchmarks/rc.zip|Benchmark|
|Covidia SPARQL Endpoint|http://covidia.acemap.info/sparql|SPARQL Endpoint|
|Covidia Search Engine|https://covidia.acemap.info/#/|Application|
|Covidia Semantic Search|https://snorql.acemap.cn/Covidia/|Application|
|QA System|https://covidia.acemap.info/#/qa|Application|

In addition, we have a sustainability plan specified for long-term maintenance of Covidia under the MIT License. The URI of each instance from Covidia is reachable, to meet the needs of Linked Open Data.

## Related Work

|                              |       Platforms       |      Subject      |           Sources          | Timeline |            Institute           |       Paper Category       | Paper Location | Paper Count | DataDump | Updating |
|:----------------------------:|:---------------------:|:-----------------:|:--------------------------:|:--------:|:------------------------------:|:--------------------------:|:--------------:|:-----------:|:--------:|:--------:|
|            [CORD-19](https://allenai.org/data/cord-19)           |        Dataset        |       Bio&Med     |      Semantic Scholar      | All time |               AI2              |             N/A            |       N/A      |   970,835   |     ✅    |     ❌    |
|           [LitCOVID](https://www.ncbi.nlm.nih.gov/research/coronavirus/)           |     Search Engine     |      Bio&Med      |           PubMed           | All time |              NCBI              |       8 Medical Class      |  Geolocations  |   349,546   |     ❌    |     ✅    |
|         [COVIDScholar](https://arxiv.org/abs/2012.03891)         |     Search Engine     |      Bio&Med      |    CORD-19 and LitCOVID    | All time | Lawrence Berkeley National Lab | 5 COVID-19 related Classes |       N/A      |   970,835   |     ❌    |     ❌    |
|      [COVID-19 Data Poral](https://www.covid19dataportal.org/)     | Data Sharing Platform |      Bio&Med      |          EuropePMC         | 2020.04~ |       the European Union       |      4 Medical Classes     |       N/A      |   959,926   |     ❌    |     ✅    |
|          [Dimensions](https://dimensions.figshare.com/articles/dataset/Dimensions_COVID-19_publications_datasets_and_clinical_trials/11961063/)          |     Search Engine     | Interdisciplinary | Subset of Digital Science  | 2020.01~ |         Digital Science        |          22 Fields         |     Country    |  1,790,530  |     ✅    |     ❌    |
|           [COVID-SEE](https://arxiv.org/abs/2008.07880)          |     Search Engine     |      Bio&Med      |           CORD-19          | All time |     University of Melbourne    |             N/A            |       N/A      |   970,835   |     ❌    |     ❌    |
|           [Docsearch](https://www.drevidence.com/)          | Medical Platform |      Bio&Med      |           PubMed           | All time |           DR.EVIDENCE          |       Medical Classes      |     Country    |  40,400,000 |     ❌    |     ✅    |
| [COVID-19 Intelligent Insight](https://covidsearch.sinequa.com/app/covid-search/#/home) |     Search Engine     |      Bio&Med      |          Preprint          | 2019.12~ |             Sinequa            |             N/A            |       N/A      |   128,000   |     ❌    |     ❌    |
|            [Covidia](https://covidia.acemap.info)           |  Search engine and KG | Interdisciplinary |     Acemap and Preprint    | 2019.12~ |              SJTU              |        22 Discipline       |       GPE      |  2,102,872  |     ✅    |     ✅    |


## Link to Wiki and DBpedia

- [ ] Coming soon (6.20)...

## Usage and Hands-on

- For [Covidia Search Engine](https://covidia.acemap.info), we have several routes for different kinds of applications.
- [Academic Paper Search Engine](https://covidia.acemap.info/#/): The users can try some keywords related to COVID-19 topics or disciplines (e.g. Vaccine in China). After starting the query, we can see the fiter and the result list on the page, and the user can click on the title to redirect to the original url, and click on the `similar paper` to find the related paper by vector search the vector is generated by the encoder trained with multiple-disciplines classification model.
- [POI Paper Search](https://covidia.acemap.info/#/mapsearch): The users can try some keywords related to COVID-19 topics or disciplines (e.g. Vaccine in China). After startign the query, we can see the paper in the area of the bounding box the user selects. The position of the papers are extracted by BERT-based method and SpaCy.
- [KG Augmented QA System](https://covidia.acemap.info/#/qa): The users can try some question related to COVID-19. On the right of the panel we can see the `tools provided`, which the users can choose for the engine for augments. If user choose `covidia_search`, the KG provided by Covidia is the augmentation, while the `bing_search` is using Bing customer search API for the augmentation.
- For [Covidia SPARQL Endpoint](http://covidia.acemap.info/sparql) and [Covidia Semantic Search](https://snorql.acemap.cn/Covidia): The user can use sparql to query the structure data from the Covidia.

Here we will provide a video for detail introduction (the video will be on before 6.20 AOE).


## Covidia Dumps and Related Code

All the supplements can be downloaded from [Google Drive](https://drive.google.com/drive/folders/1mWok37-QbLp15daoORekjDANqoek0f3N?usp=share_link)

## Acknowledgements

We thanks to the experts that provide precious annotations. They are from the Institute of Geographical Science, Natural Resources Research, Chinese Academy of Sciences, led by Chenghu Zhou. And the whole project is supported by [Deep-time Digital Earth Big Science Project](https://www.iugs.org/dde). 

## Citation

We now have a [paper](https://arxiv.org/abs/2304.07242v1) under review on ISWC Resource Track:
```bibtex
@inproceedings{covidia,
    title = "Covidia: COVID-19 Interdisciplinary Academic Knowledge Graph Construction and Application",
    author = "Cheng Deng, Jiaxin Ding, Luoyi Fu, Weinan Zhang, Xinbing Wang and Chenghu Zhou",
}
```

[schema]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/schema.nt
[ontology]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/ontology.nt
