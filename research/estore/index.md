---
layout: default
title: Research Projects
permalink: /research/estore/
---

# E-Store: an elastic in-memory OLTP system

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
