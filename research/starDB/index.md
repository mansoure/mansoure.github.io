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


## Ph.D. and Master Students Supervised

I was a co-supervisor for KAUST students, who contributed to this project.  

- [Majed Sahli](https://scholar.google.com/citations?user=cxF9uPkAAAAJ&hl=en), Ph.D on 2015
- [Ahmed El-Roby](https://scholar.google.com/citations?user=DA68vjUAAAAJ&hl=en), Master on 2011
- [Amin Allam](https://scholar.google.com/citations?user=IDVZMEIAAAAJ&hl=en), Ph.D on progress


## Publications

- Majed Sahli, Essam Mansour, Panos Kalnis: [StarDB: A Large-Scale DBMS for Strings](http://dl.acm.org/citation.cfm?id=2824082&CFID=605881404&CFTOKEN=68506341). The Proceedings of the VLDB Endowment (PVLDB) 8(12), 2015. [PDF](/publications/paper/vldb15-stardb-essam.pdf)

- Majed Sahli, Essam Mansour, Tariq Alturkestani, Panos Kalnis: [Automatic tuning of bag-of-tasks applications](http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=7113338). International Conference on Data Engineering (ICDE), 2015. [PDF](/publications/paper/icde15-APlug-essam.pdf)

- Majed Sahli, Essam Mansour, Panos Kalnis: [ACME: A scalable parallel system for extracting frequent patterns from a very long sequence](http://dl.acm.org/citation.cfm?id=2691549&CFID=605881404&CFTOKEN=68506341). VLDB Journal 23(6), 2014. [PDF](/publications/paper/vldbj14-ACME-essam.pdf)

- Majed Sahli, Essam Mansour and Panos Kalnis. [Parallel Motif Extraction from Very Long Sequences](http://dl.acm.org/citation.cfm?id=2505575&CFID=605881404&CFTOKEN=68506341). In Proceedings of the 22nd ACM International Conference on Information and Knowledge Management (CIKM), San Francisco, California, USA, 2013. [PDF](/publications/paper/cikm13-motif-essam.pdf)

- Essam Mansour, Ahmed El-Roby, Aron Ahmadia, Panos Kalnis, Ashraf Aboulnaga. [RACE: a scalable and elastic parallel system for discovering repeats in very long sequences](http://dl.acm.org/citation.cfm?id=2536214&CFID=605881404&CFTOKEN=68506341). The Proceedings of the VLDB Endowment (PVLDB), 2013. [PDF](/publications/paper/vldb13-RACE-essam.pdf)

- Essam Mansour, Amin Allam, Spiros Skiadopoulos, and Panos Kalnis. [ERA: Efficient Serial and Parallel Suffix Tree Construction for Very Long Strings](http://dl.acm.org/citation.cfm?id=2047490&CFID=605881404&CFTOKEN=68506341). In the volume 5 of Proceedings of the VLDB Endowment (PVLDB), 2011. [PDF](/publications/paper/vldb12-ERA-essam.pdf)
