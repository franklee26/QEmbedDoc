---
layout: default
title: Chimera plot
parent: Plotting
nav_order: 3
---

# Chimera plot

<p style="text-align: left;">
<span style="display: block; color: #111111; background-color: #cde4f7; border-top: 8px solid; border-top-color: #599ad6; font-family: Monospace; font-size: 1.4em;">
	QEmbed.Embed.plotChimeraFromBipartite(
	<span style = "color: #e0147d;"> showMappings = False, L = 2, M = 2, N = 2, *, left = [], right = [], isBipartite = False </span>
	)
</span>
</p>

Plots a chimera graph given a bipartite left and right sets.

<span style="font-size:1.8em;">Parameters:</span>
* **showMappings** - Boolean flag that prints mappings to console. 
* **L/M/N** - Chimera dimensions
* **left/right** - Left/right bipartite sets as an array of integers
* **isBipartite** - Boolean flag that indicates whether the input is a standard bipartite and not a virual hardware

<span style="font-size:1.8em;">Returns:</span>
* <span style = "color: #67d8ef"> None </span> - plots chimera graph
