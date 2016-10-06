---
layout: default
title: Research Projects
permalink: /research/meccano/
---

# Collaborative Data Sharing over Decentralized Graphs

This project aims to develop an efficient system and software tools to make it easy for users to share datasets with each other. In life sciences and social applications, users need to maintain their data independently of the applications consuming this data. The resource description framework (RDF) is extensively used to represent datasets on the Web. It uses a simple data model in the form of triples <subject, predicate, object>. A key feature is the ability to link two different entities from two different RDF datasets which are maintained by two local independent authorities, which could be users, research labs, or hospitals. large decentralized graphs can be easily created among a large number of RDF stores where each RDF store provides its own SPARQL endpoint. 

This radically changes the way Web applications work today, resulting in true data ownership as well as improved privacy, which are highly needed for life sciences and social applications. 
The key challenges in this decentralization and data independence are 1) develop simple and generic, yet powerful, data access mechanisms that enable developers to easily add data collaboration and sharing support to their applications, 2) providing an efficient and scalable query processing mechanism that integrates data from large decentralized graphs, 3) developing fine-grained access control and versioning mechanisms over RDF graphs.     


The first problem have been addressed by a collaboration between QCRI and MIT. Prof. Ashraf Aboulnaga, from QCRI, and  Prof. Tim Berners-Lee, from MIT, led this collaboration. We managed to develop a decentralized platform for social Web called Solid (for Social Linked Data). Solid is based on RDF and Semantic Web technologies, and it achieves the goals of providing data independence and simple yet powerful data management mechanisms. I developed Meccano, an RDF-based system that implements the Solid protocols. More details about Meccano and the Solid protocols are available in [1]. The MIT team developed [Solid.js](https://github.com/solid/solid-client), a javascript library implementing the Solid protocols. The Solid protocols guarantees efficient performance for social applications regardless these applications use Solid.js or not. However, Solid.js aims at accelerating the development lifecycle of Solid applications by writing less code. We demonstrated the Solid platform and Meccano at WWW 2016 [2].


The 2nd problem have been addressed by a collaboration between QCRI and KAUST. QCRI team includes Ashraf Aboulnaga, Mourad Ouzzani, and Essam Mansour. KAUST team includes Panos Kalnis and Ibrahim Abdelaziz. 

  



## publications

[1] Andrei Vlad Sambra, Essam Mansour, Sandro Hawke, Maged Zereba, Nicola Greco, Abdur- rahman Ghanem, Dmitri Zagidulin, Ashraf Aboulnaga, Tim Berners-Lee: Solid: A Platform for Decentralized Social Applications Based on Linked Data. Technical Report. [PDF](/research/meccano/solid_protocols.pdf)

[2] Essam Mansour, Andrei Vlad Sambra, Sandro Hawke, Maged Zereba, Sarven Capadisli, Abdurrahman Ghanem, Ashraf Aboulnaga, Tim Berners-Lee: [A Demonstration of the Solid Platform for Social Web Applications](http://dl.acm.org/citation.cfm?doid=2872518.2890529). WWW: 223-226, 2016. [PDF](/publications/paper/www16-solid-essam.pdf)
