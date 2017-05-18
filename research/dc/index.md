---
layout: default
title: Research Projects
permalink: /research/dc/
---

# The Data Civilizer System

The Data Civilizer System is to ease the pain faced in analyzing data “in the wild”. Data Civilizer is an end-to-end big data management system with components for data discovery, data integration and stitching, data cleaning, and querying data from a large variety of storage engines, running in large enterprises. The first thing needed for data discovery is a crawler, which can locate possible data sets, either inside the firewall or outside.  We propose to explore a human-assisted package that will accept hints on places to look.  It will also accept credentials to access possible databases.  Some organizations already have metadata repositories that we can hopefully access.  Using a combination of such techniques we propose to build up our registry of data sources and their contents. 

We study the problem of discovering semantic links of an enterprise knowledge graph (EKG), across hundreds of datasets from multiple ontologies. Our focus is to automatically generate an EKG that is good enough – be able to find interesting datasets via semantic links with few false positives in real-world data. We introduce a novel two-staged solution for adding semantic links to an EKG, which scales to thousands of datasets and tens of ontologies. In particular, we leverage word embeddings, which are based on neural probabilistic language models, to semantically capture similar words. We are also developing a scalable machine learning model to construct EKG on top of multiple data sources in an enterprise. We are extending our model to also rank the edges in the graph based on different task-centric objectives.


## Publications

- Raul Castro Fernandez, Dong Deng, Essam Mansour, Abdulhakim Qahtan, Ziawasch Abedjan, Ahmed Elmagarmid, Ihab F. Ilyas, Samuel Madden, Mourad Ouzzani, Michael Stonebraker, Nan Tang. [A Demo of the Data Civilizer System](/publications/paper/p1639-castro-fernandez.pdf). The International Conference on Management of Data  (SIGMOD), 2017.