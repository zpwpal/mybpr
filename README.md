# mybpr

This is a Bayesian Personlized Ranking implementation using Spark in Java

The core concept in implementation is to *persist()* RDDs as they are compute from
machine learning algorithm so if you don't, RDDs may been recomputated over iterations
. It's serious problem because with same data, machine learning algorithms will still
output different result.  
