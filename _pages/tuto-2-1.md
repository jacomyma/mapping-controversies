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
* Check what a protocol looks like

# Lorem Ipsum

Get urls for the the 931 energy conversion articles here: https://drive.google.com/file/d/1KyJyrk17581ztcJrG4Xh5vsQ678uJx6f/view?usp=sharing

Upload them to SeeAlsology

Use these settings:
- "Distance": 0 (this will ensure that the tool only gets hyperlinks from the pages you input)
- "Parent links": Not selected (this will ensure that the tool only gets links from the pages you input)
- "Take all links": Selected (this will ensure that the tool gets all links found anywhere on the pages you input)

Wait, are you sure you have used the right settings? 

Good, now you can click "Start crawling".

Observe how the network grows as the tool works its way through the 931 seed pages.

When the tool is done you can download the resulting network as a .gexf
If this did not work you can find a version of the result here: https://drive.google.com/file/d/179SeU2LSfOdgbOoqBXKcDXsoyLoshe6I/view?usp=sharing

Open the resulting network in Gephi and observe the following:

- There are much more nodes in this network than in the one you did in Tutorial 1.X on the same data. This is because SeeAlsology includes the next layer of pages that have been "seen" from the seed pages. The seed pages are coloured red and the "seen" pages are coloured blue.
- To remove the pages that are not in the seeds, we can filter the network by outdegree. Set the minimum to 1 and filter - this will ensure that only pages that have been scraped for outlinks are included.

@Mahtieu: The abouve is really hastily formulated. Feel very free, as always, to also change the wording!

# Next tutorial

[2.2. Write the protocol: scrape from one article with SeeAlsology *30 min*](../2.2/)
