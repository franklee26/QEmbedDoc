---
layout: page
title: Graph generation
permalink: docs/GraphGeneration/
nav_order : 3
has_children: true
---

# Quickstart: Easy plotting

Here's a quick introduction to some fundamental tools that you can use with QEmbed. Import the package:
```python
import QEmbed.Embed as Q
```
QEmbed can be initialised by a provided graph of the form:
```python
exampleGraph = [(1,2),(3,4),(2,4),(1,5),(2,3),(3,1),(3,5),(2,5)] # Format of an example input graph
```
where a graph is represented as a list of 2-tuples. As usual the numbers represent the node label and each tuple is an undirected edge. We initialise the object:

```python
qe = Q.Embedding(graph = exampleGraph)
```

QEmbed uses NetworkX to do graph plotting. The graph can be plotted with the call
```python
qe.plotGraph()
```
Below is our output graph:

![Example graph](https://github.com/franklee26/QEmbedDoc/blob/master/_site/assets/images/evenbetter-removebg.png?raw=true)

We can (try) to get the left and right partite sets for this graph and plot it on an appropriate Chimera topology (if it is indeed bipartite). 

```python
L, R = qe.greedyBipartiteSets()  # left and right partite sets
qe.plotChimeraFromBipartite(left = L, right = R)
```
![Example chimera](https://github.com/franklee26/QEmbedDoc/blob/master/_site/assets/images/chimera.png?raw=true)
