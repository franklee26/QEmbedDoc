---
layout: default
title: Random graph
parent: Graph Generation
nav_order: 3
---

# Random graph generation

<p style="text-align: left;">
<span style="display: block; color: #111111; background-color: #cde4f7; border-top: 8px solid; border-top-color: #599ad6; font-family: Monospace; font-size: 1.4em; height: 75px;">
	QEmbed.Embed.generateRandomGraph(
	<span style = "color: #e0147d;"> numNodes = 2, numEdges = 1, allowedRedos = 2000 </span>
	)
</span>
</p>

Method generates a fully connected undirected graph with `numNodes` nodes, `numEdges` edges. 

<span style="font-size:1.8em;">Parameters:</span>
* **numNodes** - The number of nodes desired, value is defaulted to 2 nodes.
* **numEdges** - The number of edges desired, value is defaulted to 1 edge.
* **allowedRedos** - The max number of retries allowed for trying to insert an edge in the graph, value is defaulted to 2000 max retries.

<span style="font-size:1.8em;">Returns:</span>
* <span style = "color: #e0147d"> None </span> - populates the `Embed` object with graph
