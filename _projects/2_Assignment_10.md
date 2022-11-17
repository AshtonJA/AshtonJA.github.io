---
name: Assignment 10
tools: [Python, HTML, vega-lite]
image: assets/pngs/cars.png
description: Assignment 10 plots.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Assignments 10

My two plots:


<vegachart schema-url="{{ site.baseurl }}/assets/json/Assignment10.json" style="width: 100%"></vegachart>


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/vega/vega/blob/main/docs/data/cars.json" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

