---
layout: default
title: Research Projects
---

# Research Projects

![crosscloud](/research/essamWordCloud.jpg)


## Collaborative Data Sharing over Decentralized Graphs

This project aims to develop an efficient system and software tools to make it easy for users to share datasets with each other. In life sciences and social applications, users need to maintain their data independently of the applications consuming this data. The resource description framework (RDF) is extensively used to represent datasets on the Web. It uses a simple data model in the form of triples <subject, predicate, object>. A key feature is the ability to link two different entities from two different RDF datasets which are maintained by two local independent authorities, which could be users, research labs, or hospitals. large decentralized graphs can be easily created among a large number of RDF stores where each RDF store provides its own SPARQL endpoint. 


This radically changes the way Web applications work today, resulting in true data ownership as well as improved privacy, which are highly needed for life sciences and social applications. 
The key challenges in this decentralization and data independence are 1) develop simple and generic, yet powerful, data access mechanisms that enable developers to easily add data collaboration and sharing support to their applications, 2) providing an efficient and scalable query processing mechanism that integrates data from large decentralized graphs, 3) developing fine-grained access control and versioning mechanisms over RDF graphs.     



## An Elastic in-memory OLTP System

On-line transaction processing (OLTP) database management systems
(DBMSs) often serve time-varying workloads due to daily,
weekly or seasonal fluctuations in demand, or because of rapid
growth in demand due to a company’s business success. In addition,
many OLTP workloads are heavily skewed to “hot” tuples
or ranges of tuples. For example, the majority of NYSE volume
involves only 40 stocks. To deal with such fluctuations, an OLTP
DBMS needs to be elastic; that is, it must be able to expand and
contract resources in response to load fluctuations and dynamically
balance load as hot tuples vary over time. 

This project investigated elasticity in in-memory OLTP systems, where we developed two systems
E-Store and Accordion. E-Store is designed to maintain system performance over a highly
variable and diverse load. It accomplishes this goal by balancing
tuple accesses across an elastic set of partitions. In Accordion, we explicitly considering the affinity between partitions, which indicates the frequency in which they
are accessed together by the same transactions. Accordion estimates
the capacity of a server by explicitly considering the impact
of distributed transactions and affinity on the maximum throughput
of the server.

##Large-scale Analytics on Strings

Stings are common datasets in a variety of applications such as bioinformatics,
time series analysis, clustering, text editing, log analysis, and data compression. 
There is an explosion in the production of string datasets. Analytics on strings are computationally demanding. Most of the existing solutions are not designed to utilize large computing infrastructures. Therefore, these solutions are limited to small datasets.

This project managed to develop a disk-based suffix tree construction
method, called Elastic Range (ERA), plus a rich
set of string operators that support string analytics at a large scale. 
ERA indexes the entire human genome in 19 minutes on an ordinary desktop
computer. For comparison, the fastest existing method needs 15 minutes using 1024 CPUs on an IBM BlueGene supercomputer. Our mining operators scales out to 16,384 CPUs on a supercomputer;
and supports elastic deployment in the cloud. Based on these efficient string operators, the project developed StarQL, a declarative query language for strings. StarQL is designed to support string processing that targets large datasets and large infrastructures (i.e., clusters and supercomputers). Moreover, we developed StarDB, a distributed database system that supports StarQL.  





