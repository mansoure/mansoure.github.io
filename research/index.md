---
layout: default
title: Research Projects
---

# Research Projects

## MeccanoDB: A New Architecture for the Social Web 

The project aims to radically change the way Web applications work today, resulting in true data ownership as well as improved privacy. Crosscloud provides decentralization and data independence for the social Web. At that level, the interoperability between diverse implementations is key. In addition,  we are experimenting with different architectures for client side and server-side software stacks, and different storage and query architectures. However, the priority of the work is to design the protocols. 

![crosscloud](/research/solid_arch.png)

Crosscloud Architecture. The user controls his/her identity using an RDF profile document, often stored on a pod server. The user loads an  application from an application provider. The application obtains the user's pod from the identity profile. It then follows links from the profile to discover data on the user's pod, as well as on other pods, performing authentication when needed.

Crosscloud has several goals that distinguish it from other proposals for decentralizing the social Web. For example, we are aiming at a much higher degree of data independence, that is, decoupling between data and the applications that create and consume this data.
It should be possible for end users to easily switch between applications that use the same data.
Also, Crosscloud aims to appeal to application developers by relying on Web standards and providing simple and generic, yet powerful, data access mechanisms that enable developers to easily add social features to their applications. In addition, Crosscloud is investigating the behavior and required support for applications that operate at different scale points in terms of data size or number of users whose data is accessed. For example, one of the key elements we are investigating is the extent to which query processing and Web traversal can be offloaded from client to server.

### publications
- Essam Mansour, Andrei Vlad Sambra, Sandro Hawke, Maged Zereba, Sarven Capadisli, Abdurrahman Ghanem, Ashraf Aboulnaga, Tim Berners-Lee: [A Demonstration of the Solid Platform for Social Web Applications](http://dl.acm.org/citation.cfm?doid=2872518.2890529). WWW 2016: 223-226
