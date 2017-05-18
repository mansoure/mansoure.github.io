---
layout: default
title: Research Projects
---

# Research Projects

![crosscloud](/research/essamWordCloud.jpg)


## The Data Civilizer System

The Data Civilizer System is to ease the pain faced in analyzing data “in the wild”. Data Civilizer is an end-to-end big data management system with components for data discovery, data integration and stitching, data cleaning, and querying data from a large variety of storage engines, running in large enterprises. The first thing needed for data discovery is a crawler, which can locate possible data sets, either inside the firewall or outside.  We propose to explore a human-assisted package that will accept hints on places to look.  It will also accept credentials to access possible databases.  Some organizations already have metadata repositories that we can hopefully access.  Using a combination of such techniques we propose to build up our registry of data sources and their contents. [Read more](/research/dc/)

## Managing Linked Data at Scale: Querying, Integrating, and Sharing

This project aims to develop an efficient system and software tools to make it easy for users to share datasets with each other and integrate data available at geo-distributed engines. The RDF data model allows interlinking entities from different Web sources, where each dataset is independently maintained and accessed via a SPARQL endpoint. Subsequently various applications in life sciences, government open data, decentralized social networks, and Internet of Things, which need to query RDF graphs across geo-distributed and independent endpoints, have emerged. State-of-the-art federated RDF systems usually support a small number of data sources by utilizing schema information. They often cause unnecessary data retrieval and communications, leading to poor scalability and response time; these systems cannot support the need of these emerging applications to access tens to hundreds of geo-distributed RDF datasets. [Read more](/research/meccano/)



## Elastic in-memory OLTP Systems


On-line transaction processing (OLTP) database management systems
(DBMSs) often serve time-varying workloads due to daily,
weekly or seasonal fluctuations in demand, or because of rapid
growth in demand due to a company’s business success. In addition,
many OLTP workloads are heavily skewed to “hot” tuples
or ranges of tuples. For example, the majority of NYSE volume
involves only 40 stocks. To deal with such fluctuations, an OLTP
DBMS needs to be elastic; that is, it must be able to expand and
contract resources in response to load fluctuations and dynamically
balance load as hot tuples vary over time. [Read more](/research/estore/)


## Large-scale Analytics on Strings


Stings are common datasets in a variety of applications such as bioinformatics,
time series analysis, clustering, text editing, log analysis, and data compression. 
There is an explosion in the production of string datasets. Analytics on strings are computationally demanding. Most of the existing solutions are not designed to utilize large computing infrastructures. Therefore, these solutions are limited to small datasets. [Read more](/research/starDB/)

 





