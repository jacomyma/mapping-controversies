---
permalink: /1.8/
layout: single
title: 1.8. Intro to Gephi & Visualize clusters
---

**Duration: 45 min**

[
	![Overview tuto 1.8](../assets/images/1-8.jpg)
](../assets/images/1-8.jpg)

**Goals**
* Learn how to use **Gephi**
* **Explore** a directed network
* Export a **network map**
* Annotate **clusters**

**You need**
* Gephi installed on your computer

# Data

Download this GEXF:

<center><a href="../assets/data/1-8/energy-conversion-wiki-cat-depth-1.gexf">
	<i class="fas fa-file" style="font-size:5em"></i><br>
	energy-conversion-wiki-cat-depth-1.gexf
</a><br><br></center>

It contains 787 Wikipedia pages about energy conversion connected by their hyperlinks.

Note: you can obtain a similar network by getting all the pages of the category with the notebook *[🍉&nbsp;Wikipedia category to article list](https://colab.research.google.com/github/jacomyma/mapping-controversies/blob/main/notebooks/Wikipedia_category_to_article_list.ipynb)* then feeding that list into this other notebook: *[🍣&bnsp;Wikipedia articles to hyperlinks network (slow and clean)](https://colab.research.google.com/github/jacomyma/mapping-controversies/blob/main/notebooks/Wikipedia_articles_to_hyperlinks_network_slow_and_clean.ipynb)* (10 min to compute). This gives the full category, with 3,629 articles, which is a bit big for this tutorial. Here is the [<i class="fas fa-file"></i>&nbsp;file](../assets/data/1-8/energy-conversion-wiki-cat-full.gexf) though.

# Visualize the network

Use this network: https://drive.google.com/file/d/1YT61vniGHFjaTyXhQ8PClbOYH84TTNJ2/view?usp=sharing
787 Wikipedia pages about energy conversion connected by their hyperlinks.

# Annotate
- Clusters as a way to identify subtopics of energy conversion
- Authrorities (in-degree) as a way to identify key articles per subtopic


# Next tutorial

Take a break before you get to this:

[1.9. Visualize a bipartite network *25 min*](../1.9/)
