---
permalink: /1.3/
layout: single
title: 1.3. Build a simple dashboard
---

**Duration: 15 min**

[
	![Overview tuto 1.3](../assets/images/1-2 1-3.jpg)
](../assets/images/1-2 1-3.jpg)

**Goals**
* Make a **dashboard** with Tableau

# Make a dashboard

The dataset from the last tutorial ([1.2](../1.2/)) is rich enough to create a so-called dashboard in Tableau. A dashboard is a combination of visualizations that that allow the user to filter the data by selecting parts of one visualization and observing changes to the other visualizations. This is called cross-filtering.

Let's do that by reusing the Tableau workbook from the previous tutorial and combining the visualizations we created.

How to create a dashboard:
* Click on the "New dashboard" icon at the bottom of the workbook.
* Drag the visualizations you want to combine from your list of worksheets on the left onto the dashboard canvas in the middle. 
* Select a visualization and click the small funnel-shaped icon in the top right corner to turn on filtering.
* You can now select any data point on that visualization and observe how the other visualizations on the dashboard adjust to the filtered dataset.

In the example below we combine the timeline of revisions with the ranked list of revising editors. When selecting the March 2017 spike in revisions for the "Space-based solar energy" page, the ranked list of revising editors below filters to only include data for that page and that month. Our finding from the previous tutorial that this revision spike is mainly driven by the user "Geogene" is now plain to see. 


[
	![Overview tuto 1.3](../assets/images/1-3/MappingControversies_TutorialScreenshots_FirstDashboard.svg)](../assets/images/1-3/MappingControversies_TutorialScreenshots_FirstDashboard.svg)

Rather than browsing through the page history archive right away, we can quickly make similar findings for other spikes. This makes it easier to target our investigation on Wikipedia. "What exactly was "Geogene" doing in March 2017" is a more focussed question than "what happened in March 2017". We could also, as we have done below, activate the filter on the ranked list of editors instead and select "Geogene" to see the revision timeline of that user only. This will show us that "Geogene" is 1) only active on the "Space-based solar power" page and 2) only following the initial engagement around launch costs in March 2017. 

[
	![Overview tuto 1.3](../assets/images/1-3/MappingControversies_TutorialScreenshots_FirstDashboard2.svg)](../assets/images/1-3/MappingControversies_TutorialScreenshots_FirstDashboard2.svg)



* the timeline, geographical map, the list of editors... You may have to modify your sheets for the dashboard, because there is less space.
* Use some (or all) of the [sheets as filters](https://help.tableau.com/current/pro/desktop/en-us/dashboards_create.htm#add-interactivity) to enable interactive exploration.
* Check the [help](https://help.tableau.com/current/pro/desktop/en-us/dashboards_create.htm#create-a-dashboard-and-add-or-replace-sheets) if you're lost.

It may look like this:
[
	![Dashboard](../assets/images/1-3/Dashboard.png)
](../assets/images/1-3/Dashboard.png)

Or like that:
[
	![Dashboard](../assets/images/1-3/Dashboard-2.png)
](../assets/images/1-3/Dashboard-2.png)

# Explore the data by filtering the dashboard 

Explore the data with the dashboard. Filter in different ways to explore different aspects. Each question may require a specific kind of filtering, and therefore a dashboard with specific sheets.

# Make an annotated visualization

Pick a question that you can answer with the dashboard, and use it to annotate the visualization.

Example of questions you may use:
* Are there editors in Denmark? If so, who are they?
* Are there editors who edited both pages?
* Who edited during a spike?

You may draw inspiration from this:

[
	![Dashboard](../assets/images/1-3/Dashboard-3.png)
](../assets/images/1-3/Dashboard-3.png)

[
	![Dashboard](../assets/images/1-3/Dashboard-4.png)
](../assets/images/1-3/Dashboard-4.png)

# Documents produced

Keep somewhere, for sharing, the following document:
* The annotated visualization (JPEG or PNG)

# Next activity

[<i class="fas fa-forward"></i>&nbsp;1.4. A small-multiple with words *(30 min)*](../1.4/)

---

### Additional resources

* This [intro to Tableau in 23 minutes](https://www.youtube.com/watch?v=jEgVto5QME8) we mentionned before shows how to create a dashboard.