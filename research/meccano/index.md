---
layout: default
title: Research Projects
permalink: /research/meccano/
---

# Collaborative Sharing and Data Integration over Decentralized Graphs

This project aims to develop an efficient system and software tools to make it easy for users to share datasets with each other and integrate data available at geo-distributed engines. The RDF data model allows interlinking entities from different Web sources, where each dataset is independently maintained and accessed via a SPARQL endpoint. Subsequently various applications in life sciences, government open data, decentralized social networks, and Internet of Things, which need to query RDF graphs across geo-distributed and independent endpoints, have emerged. State-of-the-art federated RDF systems usually support a small number of data sources by utilizing schema information. They often cause unnecessary data retrieval and communications, leading to poor scalability and response time; these systems cannot support the need of these emerging applications to access tens to hundreds of geo-distributed RDF datasets.


This project mainly addresses these limitations and presents Lusail, a scalable and efficient federated RDF engine for querying large-scale graphs across geo-distributed endpoints. Lusail achieves scalability and low query response time through optimizations at compile and run times. At compile time, we use a novel locality-aware query decomposition [1] that maximizes the number of query triple patterns sent together to a source based on the actual location of the instances satisfying these triple patterns. At run time, we use selectivity- aware and parallel query execution techniques to reduce net- work latency and to increase parallelism by delaying the execution of subqueries expected to return large results. We evaluate Lusail using real data and synthetic benchmarks, with sizes up to billions of triples on an in-house cluster and a geo-distributed public cloud. We show that Lusail outperforms state-of-the-art systems by orders of magnitude in terms of scalability and response time. Lusail is demonstrated at SIGMOD 2017 [2]. A full technical report about Lusail is available at [3].    

  
We also addressed the data sharing problem in a short collaboration between QCRI and MIT. Prof. Ashraf Aboulnaga, from QCRI, and  Prof. Tim Berners-Lee, from MIT, led this collaboration. We managed to develop a decentralized platform for social Web called Solid (for Social Linked Data). Solid is based on RDF and Semantic Web technologies, and it achieves the goals of providing data independence and simple yet powerful data management mechanisms. I developed Meccano, an RDF-based system that implements the Solid protocols. More details about Meccano and the Solid protocols are available in [4]. The MIT team developed [Solid.js](https://github.com/solid/solid-client), a javascript library implementing the Solid protocols. The Solid protocols guarantees efficient performance for social applications regardless these applications use Solid.js or not. However, Solid.js aims at accelerating the development life-cycle of Solid applications by writing less code. We demonstrated the Solid platform and Meccano at WWW 2016 [5].



## publications

[1] Ibrahim Abdelaziz, Essam Mansour, Mourad Ouzzani, Ashraf Aboulnaga, Panos Kalnis. Query Optimizations Over Decentralized RDF Graphs. IEEE International Conference on Data Engineering (ICDE), 2017.

[2] Essam Mansour, Ibrahim Abdelaziz, Mourad Ouzzani, Ashraf Aboulnaga, Panos Kalnis. A Demonstration of Lusail – Querying Linked Data at Scale. The International Conference on Management of Data (SIGMOD), 2017.

[3] Ibrahim Abdelaziz, Essam Mansour, Mourad Ouzzani, Ashraf Aboulnaga, Panos Kalnis. Lusail: A System for Querying Linked Data at Scale. Technical Report.

[4] Andrei Vlad Sambra, Essam Mansour, Sandro Hawke, Maged Zereba, Nicola Greco, Abdur- rahman Ghanem, Dmitri Zagidulin, Ashraf Aboulnaga, Tim Berners-Lee: Solid: A Platform for Decentralized Social Applications Based on Linked Data. Technical Report. [PDF](/research/meccano/solid_protocols.pdf)

[5] Essam Mansour, Andrei Vlad Sambra, Sandro Hawke, Maged Zereba, Sarven Capadisli, Abdurrahman Ghanem, Ashraf Aboulnaga, Tim Berners-Lee: [A Demonstration of the Solid Platform for Social Web Applications](http://dl.acm.org/citation.cfm?doid=2872518.2890529). WWW: 223-226, 2016. [PDF](/publications/paper/www16-solid-essam.pdf)
