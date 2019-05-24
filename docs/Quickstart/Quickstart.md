---
layout: page
title: Quickstart
permalink: docs/Quickstart/
nav_order : 2
has_children: true
---

# Quickstart

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
