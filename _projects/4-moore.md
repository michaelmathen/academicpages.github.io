---
title: "Moore"
excerpt: "Does a combinatorial search to find Moore Graphs that satisfy the Hoffman–Singleton theorem.  <br/><img src='/images/petersen_graph.png'>"
permalink: /projects/moore
collection: projects
---
This project attempts to find all of the Moore Graphs with girth 5. 
According to Wikipedia:
The Hoffman–Singleton theorem states that any Moore graph with girth 5 must have degree 2, 3, 7, or 57. The Moore graphs are:
* The complete graphs  K_n  on n > 2 nodes. (diameter 1, girth 3, degree n-1, order n)
* The odd cycles  C_{2n+1} . (diameter n, girth 2n+1, degree 2, order 2n+1)
* The Petersen graph. (diameter 2, girth 5, degree 3, order 10)
* The Hoffman–Singleton graph. (diameter 2, girth 5, degree 7, order 50)
* A hypothetical graph of diameter 2, girth 5, degree 57 and order 3250; it is currently unknown whether such a graph exists.
Unlike all other Moore graphs, Higman proved that the unknown Moore graph cannot be vertex-transitive.


This code should be pretty easy to compile as there are no requirements on any libraries outside of the standard right now.
I was going to accelerate this with cuda and omp, but a factor of 100 increase in speed wouldn't really help you with the 57
degree graph and would be unnoticeable with the 7 or 3 as they are already extremely fast. 
You will probably have to change the CC variable in the makefile to fit your system and you will need a c++ compiler that is 
modern enough to support C++11 features. 

[Github link](https://github.com/michaelmathen/)
