---
permalink: /2.5/
layout: single
title: "2.5. Do your own network from a category"
---

**Duration: 45 min + 45 min**

**Goals**
* Activate your knowledge
* Make your own network map from scratch:
	* from **sourcing**
	* to **harvesting**,
	* **visualization**,
	* **annotation**,
	* and **writing the protocol**.
* Contribute to your **own group project**, at least as a test.

# Task

It is now time to go through the whole process you have just learned, but on your own data set and for your own project.

1. Choose a Wikipedia **category**
1. Source a list of its Wikipedia **articles**
1. **Harvest** at least 2 networks
1. **Analyze and visualize** them
1. **Annotate** your network maps
1. Write the **visual protocols**

# Advice and comments

* **Help each other!**
* Check the **[list of notebooks](../nb/)**.
* Pay attention to the **quality of the sourcing** (the list of articles). The better, the easier the work of analyzing it: check that the articles are actually related to your topic.
* **What size** for the sourcing (articles list)?
	* Not too small, not too big: between 100 and 5000, but it also depends.
	* If the subsequent harvesting makes your data bigger (e.g., articles and editors), prefer smaller lists (max level low).
	* If not (e.g., hyperlinks network), you can probably visualize a network of thousands of nodes, and more if you filter it.
	* If you have two, source multiple lists (same category, but at different levels).
* During **network analysis**, consider:
	* Filtering your network
	* Computing centrality metrics, then annotating the important nodes
	* Computing modularity clustering, them annotating the clusters
	* Reflecting on the edges' direction and weight, if any.
* You may make **multiple network maps** for the same network.
* You may make **multiple annotated visualizations** for a same network map.
* Prioritize **clarity** in your visualizations and visual protocols.
* If it makes more sense, you may **join your protocols** into a single diagram.
* **Take risks!** This is a good occasion to try something uncertain. Data science is a bet, it's exploration.
* **Take a break** at some point. You have a time slot of approximatively 1 hour and 45 minutes, including a 15 minutes break.

# Documents produced

Keep somewhere, for sharing, the following documents:
* The images of the annotated network maps (JPEG or PNG)
* The image(s) of the visual protocol(s) (JPEG or PNG)

# Share your work

Your teachers will provide you with a Padlet where you can share your annotated maps and visual protocols. Make sure that you put them up before you have lunch.

# Next tutorial

🥩 Lunch break: take forces!

The afternoon starts with this:

[<i class="fas fa-forward"></i>&nbsp;2.6. Follow the protocol: words, from manual curation to Tableau *(45 min)*](../2.6/)

---


### Tools for getting similar data (networks in GEXF or GDF format) from other sources:

* Networks of users, hashtags, or emojis from Twitter with the [Twitter Streaming Importer plugin for Gephi](https://github.com/seinecle/gephi-tutorials/blob/master/src/main/asciidoc/en/plugins/twitter-streaming-importer-en.adoc). Takes a list of words/#tags or a list of users as input.
* Networks of YouTube channels or YouTube videos connected by their relatedness (as meassured by the algorithmic recommendations) with the [YouTube Data Tools](https://tools.digitalmethods.net/netvizz/youtube/). Takes a list of video or channel ID's as input.
* Networks of scientific publications connected through keywords or citations with [ScienceScape](http://medialab.github.io/sciencescape/). Takes a full export from Scopus as input.

### Relation to the course readings

* The process of getting data through scraping, crawling and calling APIs is covered in **Chapter 6: Collecting and curating digital records** of *Venturini, T. & Munk, A.K. (2021). Controversy Mapping: A Field Guide.*
* The intricacies of Wikipedia and the different ways in which the platform may be reappropriated for controversy analysis are covered in *Weltevrede, E., & Borra, E. (2016).* **Platform affordances and data practices: The value of dispute on Wikipedia**
*Big Data & Society, 3(1).*
* The principles and concepts of Visual Network Analysis (VNA) are covered in **Chapter 2: What is visual network analysis** in *Jacomy, M. (2021). Situating Visual Network Analysis*
* And in **Chapter 7: Visual network analysis** in *Venturini, T. & Munk, A.K. (2021). Controversy Mapping: A Field Guide*
* An example of how to visualize and annotate the same network of wikipedia articles in different ways is described in **Figures 62-65** of *Venturini, T. & Munk, A.K. (2021). Controversy Mapping: A Field Guide*:

[
	![CM Figure 62](https://medihal.archives-ouvertes.fr/hal-03227401/image)
](https://medihal.archives-ouvertes.fr/hal-03227401/image)
*Two renderings of a network of Wikipedia pages related to the Green Revolution. Top, density heatmap and structural holes; bottom, clusters and sub-clusters*

[
	![CM Figure 63](https://medihal.archives-ouvertes.fr/hal-03227404/image)
](https://medihal.archives-ouvertes.fr/hal-03227404/image)
*Central (continuous contour) and bridging (dotted line) nodes in the Green Revolution networks*

[
	![CM Figure 64](https://medihal.archives-ouvertes.fr/hal-03227411/image)
](https://medihal.archives-ouvertes.fr/hal-03227411/image)
*Authorities (left) and hubs (right) of the Green Revolution network*

[
	![CM Figure 65](https://medihal.archives-ouvertes.fr/hal-03227419/image)
](https://medihal.archives-ouvertes.fr/hal-03227419/image)
*The Green Revolution network colored according to our manual thematic classification of Wikipedia pages*