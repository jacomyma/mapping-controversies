---
permalink: /2.1/
layout: single
title: "2.1. Follow the protocol: scrape a network with SeeAlsology"
---

**Duration: 15 min**

[
	![Overview tuto 2.1](../assets/images/2-1 2-2.jpg)
](../assets/images/2-1 2-2.jpg)

**Goals**
* Discover **SeeAlsology**
* Export a network
* Check what a **protocol** looks like

# Case

We still stick to the case of energy conversion, using Wikipedia as the main data source.

# Protocol

Take a close look at this protocol:
[
	![Protocol](../assets/images/2-1/Protocol_Tutorial2-1.svg)
](../assets/images/2-1/Protocol_Tutorial2-1.svg)

* The protocol summarizes all the information one needs to know to understand the data and/or reproduce the experiment
* It mentions mentions the tools, but also the **most relevant settings**. Notably, when data have been removed.
* The main purpose of the protocol is to **provide context** to interpret the results.
* How to know what to feature in the protocol? Anything that is necessary to **reproducing** the process. Because then it means that it partially determined the result, and thus is necessary to understand it.

<div class="notice--info">In the following tutorials, we will alternate between following protocols and writing them. Ultimately, the goal is to learn how to write a protocol, as an important and necessary part of data-driven stories.</div>

# Data

Download this CSV:

<center><a href="../assets/data/2-1/wikipedia-URL-energy-conversion.csv">
	<i class="fas fa-file-csv" style="font-size:5em"></i><br>
	wikipedia-URL-energy-conversion.csv
</a><br><br></center>

It contains 139 Wikipedia page URLs about energy conversion (no subcategories included). As you have seen, this file is the starting point of the protocol.

<div class="notice">Contrary to a similar file we have seen in a previous tutorial, this one contains page URLs, not titles. It also has no header. This is what SeeAlsology needs.</div>

# SeeAlsology

[SeeAlsology](https://densitydesign.github.io/strumentalia-seealsology/) is an online tool that builds a network of Wikipedia pages and their hyperlinks. By default, it only looks at the hyperlinks in the "See also" section, hence its name. But it has a setting to grab all hyperlinks (we will use it).

* Open [SeeAlsology](https://densitydesign.github.io/strumentalia-seealsology/) in a browser
* Open the CSV file in a spreadsheet or text editor, and copy-paste the list of URLs into SeeAlsology
* Use these settings:
	* ```Distance```: ```0``` (this will ensure that the tool only gets hyperlinks from the pages you input)
	* ```Parent links```: ```Unchecked``` (this will ensure that the tool only gets links from the pages you input)
	* ```Take all links```: ```Checked``` (this will ensure that the tool gets all links found anywhere on the pages you input)

Wait, **are you sure you have used the right settings?**

Good, now you can click on ```Start crawling```.

Observe how the network grows as the tool works its way through the 139 seed pages.

When the tool is done you can download the resulting network as a .GEXF file. If this did not work you can find a version of the result [<i class="fas fa-file"></i>&nbsp;here](../assets/data/2-1/seealsology-network.gexf).

# Visualize in Gephi

Open the resulting network in Gephi and observe the following:
* There are much more nodes in this network than in the one you did in [tutorial 1.8](../1.8/) on a similar dataset. This is because SeeAlsology includes the next layer of pages that have been "seen" from the seed pages. The seed pages are coloured red and the "seen" pages are coloured blue.
* To remove the pages that are not in the seeds, we can filter the network by outdegree. Set the minimum to 1 and filter - this will ensure that only pages that have been scraped for outlinks are included.

# Check the protocol

Check that you have followed the protocol. **You do not have to do the "ANNOTATE" part** in this tutorial and those that come after, except the last one. Keep in mind, however, that featuring the annotation in the protocol is a good practice.

# Next tutorial

[<i class="fas fa-forward"></i>&nbsp;2.2. Write the protocol: scrape from one article with SeeAlsology *(30 min)*](../2.2/)
