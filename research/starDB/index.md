---
layout: default
title: Research Projects
permalink: /research/starDB/
---

# Large-scale Analytics on Strings

Stings are common datasets in a variety of applications such as bioinformatics,
time series analysis, clustering, text editing, log analysis, and data compression. 
There is an explosion in the production of string datasets. Analytics on strings are computationally demanding. Most of the existing solutions are not designed to utilize large computing infrastructures. Therefore, these solutions are limited to small datasets. 

This project managed to develop a disk-based suffix tree construction
method, called Elastic Range (ERA), plus a rich
set of string operators that support string analytics at a large scale. 
ERA indexes the entire human genome in 19 minutes on an ordinary desktop
computer. For comparison, the fastest existing method needs 15 minutes using 1024 CPUs on an IBM BlueGene supercomputer. Our mining operators scales out to 16,384 CPUs on a supercomputer;
and supports elastic deployment in the cloud. Based on these efficient string operators, the project developed StarQL, a declarative query language for strings. StarQL is designed to support string processing that targets large datasets and large infrastructures (i.e., clusters and supercomputers). Moreover, we developed StarDB, a distributed database system that supports StarQL.