---
name: Assignment 10
tools: [Python, HTML, vega-lite]
image: assets/pngs/Assignment10GraphPic.png
description: Assignment 10 plots.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Assignments 10

My two plots (Click on the bar graph!) :


<vegachart schema-url="{{ site.baseurl }}/assets/json/Assignment10.json" style="width: 100%"></vegachart>


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/AshtonJA/AshtonJA.github.io/blob/main/python_notebooks/DataViz_Assignment10.ipynb" text="The Analysis" %}
</div>

