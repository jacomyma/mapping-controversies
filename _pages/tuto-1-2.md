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

[
	<i class="fas fa-file-csv" style="font-size:5em"></i><br>
	wikipedia-edits-tuto-1.2.csv{: .text-center}
](../assets/data/1-2/wikipedia-edits-tuto-1.2.csv)

It contains the list of edits (i.e. revisions) for these two pages. It has been produced by feeding this [<i class="fas fa-file-csv"></i> file](../assets/data/1-2/wikipedia-articles-tuto-1.2.csv) into this notebook: [🍹 Wikipedia articles to edits list](https://colab.research.google.com/github/jacomyma/mapping-controversies/blob/main/notebooks/Wikipedia_articles_to_edits_list.ipynb), but we will see that in the [tuto 1.6](../1.6/).

# Load your data into Tableau

Same Wikipedia pages as previous, but this time we look at revisions: https://drive.google.com/file/d/1kBNI3wiVEYKjgLDjxkzvo1RovrhPwo7d/view?usp=sharing

Note: we can make a point out of the fact that this time there are more columns to choose from and so the complexity goes up.

# Visualize the data as a timeline of revisions


# Visualize the data as a ranked list of revising editors 

# Visualize the data as a geographical map of anonymous editors

# Make an annotated visualization of the timeline of revisions

Helpful pointers for the comparison:
- Not a lot of revision activity in the thorium article in October 2016. So even though we have a lot of page views - i.e. public interest in the topic driven by outside events - it does not correspond to a big change in how the article is written. No new content is added or reverted in this period.
- Similar for the November 2015 spike in pages views on the solar article. Does not correspond to a spike in revisions. And for the June 2019 spike in page views. It just confirms that revisions tell a different story than page views.  When the substance of the debate is changing, pages get revised, but that is not necessarily the same as the general public taking note and going to read the article.

# Next tutorial

You deserve a break! Then head for the next tutorial:

[<i class="fas fa-forward"></i> 1.3. Build a simple dashboard *(15 min)*](../1.3/)

---

