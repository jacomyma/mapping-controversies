---
permalink: /2.2/
layout: single
title: "2.2. Write the protocol: scrape from one article with SeeAlsology"
---

**Duration: 30 min**

[
	![Overview tuto 2.2](../assets/images/2-1 2-2.jpg)
](../assets/images/2-1 2-2.jpg)

**Goals**
* **Harvest your own network** with SeeAlsology
* Explore it with Gephi
* **Write your own protocol**

# Case

**Your choice!** Pick one Wikipedia article. Prioritize a topic that:
* You know about
* You are curious about
* Is linked to a controversy you want to map
* An article that is not too long, *or* that has a good "See also" section.

*Still no idea? Try [this one](https://en.wikipedia.org/wiki/Copenhagen).*

# Harvest a network with SeeAlsology

* Open [SeeAlsology](https://densitydesign.github.io/strumentalia-seealsology/)
* Copy-paste the URL of the Wikipedia article of your choice
* Harvest a network

You should ask yourself the following questions, probably in this order:
* Do I want to harvest links backwards (pages that cite my article, and so on)? If so, enable ```Parent links```.
* Do I want all the links, or just the "See also"? Check the ```Take all links``` setting.
* How far should I go? That is, what ```Distance```? **Tip:** start with small distances first.
* Do I want to filter the nodes later on in Gephi? Possibly because there are too many poorly connected nodes...

These questions have no obvious answer. They depend on your article. Some articles do not have a "See also" section, so it forces you to take all links. Some articles cite many other articles, so the network grows too fast and you must pick a low distance. Some articles have many parent articles, some none, etc.

*How to decide:* Look at a network size that is feasible. Too big, and it will get slow or impossible to work with your network. Too small, and there will be nothing to interpret. Aim for a size that you are comfortable with. Maybe 100 to 1,000 nodes? It also depends on the performance of your computer!

***Remark:** By definition, a distance of 0 gives you just your starting article. Similarly, a distancce of 1 gives you the starting article and its neighbors, but not the links between them (a star-shaped network). So you probably need a distance of 2 or more.*

**Tip:** If your starting page has enough "See also" links, then you do not take all the links, you might get a nice network with high distances (3 or more).

**Tip:** If you harvested all the links, then you probably need to filter your network in Gephi.

This is the network obtained for the article [Copenhagen](https://en.wikipedia.org/wiki/Copenhagen) with a depth of 3, with parent links, see-also links only. Here is the [<i class="fas fa-file"></i>&nbsp;GEXF](../assets/data/2-2/see-also-copenhagen.gexf), by the way.

[
	![See also Copenhagen](../assets/images/2-2/see-also-copenhagen.png)
](../assets/images/2-2/see-also-copenhagen.png)

# Visualize in Gephi

* Export the GEXF from SeeAlsology (under the drop-down button ```Download```).
* Visualize it in Gephi. You may have to filter out some nodes if it's too hairy...
* Export the PNG (no need to annotate, though)

# Write the protocol

Using Google Slides, write the protocol of the image you have produced. **It must feature the methodological decisions you have made in SeeAlsology.**

# Deliverables

Keep somewhere, for sharing, the following documents:
* The image of the network map (PNG)
* The image of the protocol (PNG)

# Next tutorial

[<i class="fas fa-forward"></i>&nbsp;2.3. Follow the protocol: co-reference network from a category *(15 min)*](../2.3/)

...but first, let's take a break.