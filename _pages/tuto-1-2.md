---
permalink: /1.2/
layout: single
title: 1.2. Visualize a different dataset with Tableau
---

**Duration: 15 min**

[
	![Overview tuto 1.2](../assets/images/1-2 1-3.jpg)
](../assets/images/1-2 1-3.jpg)

**Goals**
* Check that different data tell a different story
* Try different visual models for different aspects of data
* Make another annotated visualization

# Case

We still focus on the topic of *energy conversion* using the same two Wikipedia articles:
* [Space-based solar power](https://en.wikipedia.org/wiki/Space-based_solar_power)
* [Thorium-based nuclear power](https://en.wikipedia.org/wiki/Thorium-based_nuclear_power)

# Data

Download this CSV:

<center><a href="../assets/data/1-2/wikipedia-edits-tuto-1.2.csv">
	<i class="fas fa-file-csv" style="font-size:5em"></i><br>
	wikipedia-edits-tuto-1.2.csv
</a><br><br></center>

It contains the list of edits (i.e. revisions) for these two pages. It has been produced by feeding this [<i class="fas fa-file-csv"></i> file](../assets/data/1-2/wikipedia-articles-tuto-1.2.csv) into this notebook: [🍹&nbsp;Wikipedia articles to edits list](https://colab.research.google.com/github/jacomyma/mapping-controversies/blob/main/notebooks/Wikipedia_articles_to_edits_list.ipynb), but we will see that in the [tutorial 1.6](../1.6/).

# Load your data into Tableau

Upload the data like in [tutorial 1.1](../1.1/), and take a look at it. There are more columns to choose from, so the complexity goes up.

[
	![Data table](../assets/images/1-2/data-table.png)
](../assets/images/1-2/data-table.png)

# Visualize a timeline of revisions

Simple things first. The idea is to look at the revision history of these pages, like we have done previously. When were they *edited* the most? It may look like this:

[
	![Timeline of revisions](../assets/images/1-2/tableau-timelime-revisions-2.png)
](../assets/images/1-2/tableau-timelime-revisions-2.png)

Remark that although this visualization looks like that of [tutorial 1.1](../1.1/), the data represent something completely different: revisions (not views). Which begs these questions:
* Is there a correlation between the number of views and the number of edits over time?
* Should we expect such correlation? Why or why not?

# Visualize a ranked list of revising editors 

<div class="notice">**Watch out!** Create each different visualization in a different sheet, so that we can combine them in the next tutorial.</div>

The data are richer, which brings opportunities. As we have a column with the usernames of the editors, we can look into this. Let's visualize if some editors have contributed more than others. It may look like this:

[
	![Ranked editors](../assets/images/1-2/tableau-ranked-list-editors.png)
](../assets/images/1-2/tableau-ranked-list-editors.png)


# Visualize a geographical map

We can also wonder where the editors live. It may look like this:
[
	![Map](../assets/images/1-2/tableau-geographical-map.png)
](../assets/images/1-2/tableau-geographical-map.png)

Remark: not all editors have latitude and longitude data. You can see that in the data table. So this map is not representative of the whole data. Tableau tells you, in the visualization, that some of the data points were not placed in the map. Did you see it?

# Annotated the timeline of revisions

Annotate the visualization like [previously](../1.1/):
* Export a static image from Tableau
* Import it into Google Slides
* Annotate the important features of the visualization
* Export the annotated image

**Later on, you will upload the annotated image to share with the other students.**

Here is some help about interpreting the results:
- Not a lot of revision activity in the thorium article in October 2016. So even though we have a lot of page views - i.e. public interest in the topic driven by outside events - it does not correspond to a big change in how the article is written. No new content is added or reverted in this period.
- Similar for the November 2015 spike in pages views on the solar article. Does not correspond to a spike in revisions. And for the June 2019 spike in page views. It just confirms that revisions tell a different story than page views.  When the substance of the debate is changing, pages get revised, but that is not necessarily the same as the general public taking note and going to read the article.

# Next tutorial

You deserve a break! Then head for the next tutorial:

[<i class="fas fa-forward"></i>&nbsp;1.3. Build a simple dashboard *(15 min)*](../1.3/)

