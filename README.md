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

**Notice: Our datasets has been ready on May 22th**

 
## Covidia Dumps and Related Code

All the supplements can be downloaded from [Google Drive](https://drive.google.com/drive/folders/1mWok37-QbLp15daoORekjDANqoek0f3N?usp=share_link)

## TODO
**Notice: More detail about Covidia will be released soon!!!**

## Citation

We now have a [paper](https://arxiv.org/abs/2304.07242v1) under review on ISWC Applied Research Track:
```bibtex
@inproceedings{covidia,
    title = "Covidia: COVID-19 Interdisciplinary Academic Knowledge Graph Construction and Application",
    author = "Cheng Deng, Jiaxin Ding, Luoyi Fu, Weinan Zhang, Xinbing Wang and Chenghu Zhou",
}
```

[schema]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/schema.nt
[ontology]: https://dataset.acemap.info/covidia/covidia-dump-v1-05-22/ontology.nt
