---
permalink: /2.3/
layout: single
title: "2.3. Follow the protocol: co-reference network from a category"
---

**Duration: 15 min**

[
	![Overview tuto 2.3](../assets/images/2-3.jpg)
](../assets/images/2-3.jpg)

**Goals**
* Check **two new Jupyter notebooks**
* Check how **Wikipedia categories** can be repurposed to get data
* **Harvest** a co-reference network from a Wikipedia category
* Follow a more complex protocol

# Datum

The only data we need is this single bit of text:

```
Category:Energy conversion
```

This is just the title of the [Wikipedia category on energy conversion](https://en.wikipedia.org/wiki/Category:Energy_conversion). It's nevertheless a *datum* (singular of data)!

A category on Wikipedia is a collection of pages about a specific topic curated by the editors. Notice that there are subcategories inside the category. This means that some pages are found directly in the category, while other pages that might still be topically relevant are found at deeper levels of subcategories. Level 0 would be pages found directly in the category, while level 2 would be pages found inside a subcategory of a subcategory of the category. We will make use of that to control the harvest below.

# Protocol

Here is the protocol (you can skip the annotation as you have already done something similar in Tutorial 1.10):

[
	![Overview tuto 2.3](../assets/images/2-3/Protocol_Tutorial2-3.svg)
](../assets/images/2-3/Protocol_Tutorial2-3.svg)


Follow these instructions:
* Harvest the Wikipedia articles listed in a Wikipedia category
	* The Wikipedia category is *energy conversion*
	* Use a ```max level``` of 0 (harvest no subcategories)
	* Use the following notebook: [🍉&nbsp;Wikipedia category to article list](https://colab.research.google.com/github/jacomyma/mapping-controversies/blob/main/notebooks/Wikipedia_category_to_article_list.ipynb)
	* You should obtain a [<i class="fas fa-file-csv"></i> CSV list](../assets/data/2-3/wikipedia-articles.csv) of 139 articles
* Harvest a co-reference network (articles connected when they share one or more references)
	* Use the list of articles as an input
	* Use the following notebook: [🫕&nbsp;Wikipedia articles to co-reference network](https://colab.research.google.com/github/jacomyma/mapping-controversies/blob/main/notebooks/Wikipedia_articles_to_co_reference_network.ipynb)
	* You should obtain a [<i class="fas fa-file"></i> GEXF](../assets/data/2-3/wikipedia-articles-coreference-network.gexf)
* Visualize the GEXF in Gephi
	* Export the network map as an image

If you've done it all, bravo! You have discovered two new notebooks that you can use later on. The network map you have produced is basically the same as that of [tutorial 1.10](../1.10/), except it has less nodes. If you have more time, you can get the big network: just set ```max level``` at 2. It's just a bit long for the time we have...

# Documents produced

Keep somewhere, for sharing, the following document:
* The (unannotated) network map (JPEG or PNG)

# Next activity

[<i class="fas fa-forward"></i>&nbsp;2.4. Write the protocol: Article-editor network from a category *(30 min)*](../2.4/)

---

### Relation to the course readings

* The process of getting data through scraping, crawling and calling APIs is covered in **Chapter 6: Collecting and curating digital records** of *Venturini, T. & Munk, A.K. (2021). Controversy Mapping: A Field Guide.*
* The intricacies of Wikipedia and the different ways in which the platform may be reappropriated for controversy analysis are covered in *Weltevrede, E., & Borra, E. (2016).* **Platform affordances and data practices: The value of dispute on Wikipedia**
*Big Data & Society, 3(1).*
* The principles and concepts of Visual Network Analysis (VNA) are covered in **Chapter 2: What is visual network analysis** in *Jacomy, M. (2021). Situating Visual Network Analysis*
* And in **Chapter 7: Visual network analysis** in *Venturini, T. & Munk, A.K. (2021). Controversy Mapping: A Field Guide*

### Tools for getting similar data (networks in GEXF or GDF format) from other sources:

* Networks of users, hashtags, or emojis from Twitter with the [Twitter Streaming Importer plugin for Gephi](https://github.com/seinecle/gephi-tutorials/blob/master/src/main/asciidoc/en/plugins/twitter-streaming-importer-en.adoc). Takes a list of words/#tags or a list of users as input.
* Networks of YouTube channels or YouTube videos connected by their relatedness (as meassured by the algorithmic recommendations) with the [YouTube Data Tools](https://tools.digitalmethods.net/netvizz/youtube/). Takes a list of video or channel ID's as input.
* Networks of scientific publications connected through keywords or citations with [ScienceScape](http://medialab.github.io/sciencescape/). Takes a full export from Scopus as input.
