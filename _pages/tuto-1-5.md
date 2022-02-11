---
permalink: /1.5/
layout: single
title: 1.5. Harvest a dataset
---

**Duration: 15 min**

[
	![Overview tuto 1.5](../assets/images/1-5.jpg)
](../assets/images/1-5.jpg)

**Goals**
* *Harvest* a dataset from an online source

# Harvest a dataset

We will use Toolforge [PageViews](https://pageviews.toolforge.org) to harvest a dataset. The goal is to harvest the same dataset we have used to build the timeline of page views in [tutorial 1.1](../1.1/).

* Go to [PageViews](https://pageviews.toolforge.org)
* Visualize the data for the two following Wikipedia articles:
	* ```Space-based solar power```
	* ```Thorium-based nuclear power```
* Use the right settings:
	* The ```Dates``` should be from 01/07/2015 to today (we used 06/02/2022)
	* The ```Date type``` should be ```Daily```. Indeed, Tableau can aggregate into months or years easily, so the more precise data is just better.
* Download the dataset by clicking on the ```Download``` drop-down menu and selecting ```CSV```.

# Visualize

Open the dataset into Tableau and check that it works. Can you visualize it at the day level using bars? It may look like this:

[
	![Timeline](../assets/images/1-5/timeline.png)
](../assets/images/1-5/timeline.png)

<div class="notice--info"><b>TIP:</b> if the bars look grey, that is because they are so thin that we only see their grey border. If you want to remove that border, click on the <code>Color</code> button in the <code>Marks</code> panel and set <code>Borders</code> to <code>None</code>.</div>

No need to annotate this time (you've done it already in the [first tutorial](../1.1/)).

# Documents produced

This time, none!

# Next tutorial

[<i class="fas fa-forward"></i>&nbsp;1.6. Harvest data with a notebook *(30 min)*](../1.6/)

# Tools for getting similar data (CSV format with timestamps) from other sources:
* [Search interest over time with Google Trends](https://trends.google.com/trends/?geo=DK). Note that this can be filtered to geographical regions or other Google platforms such as YouTube, News or Shopping.
* [Acitivity on Twitter over time with Social Bearing](https://socialbearing.com/search/user). Note that the input can be a single user handle or a hashtag, but that hashtag activity is hard to get more than a week back.
* [Publication activity around a topic over time in scientific journals with Scopus](https://www.scopus.com/). Note that you will need to use your university login.
* [Activity on public Facebook pages over time with FacePager](https://github.com/strohne/Facepager). Note that you will need to install the software.

