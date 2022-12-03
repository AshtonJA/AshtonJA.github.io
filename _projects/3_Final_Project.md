---
name: Efficiency of Electric Vehicles in Washington State Cities
tools: [Python, HTML, vega-lite]
image: assets/pngs/WashingtonDL.png
description: An in-depth evaluation of electric vehicles registered in Washington State.
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Efficiency of Electric Vehicles in Washington State Cities

Published by: Ashton Anaya

As electric vehicles continue to become more popular, one of the most pressing issues for potential buyers is the limited range they are able to travel before having to be recharged.
 Using a dataset published by the Washington State Department of Licensing we can evaluate what the current state of electric vehicles looks like
in reality. The dataset I'll be using in this examination is published on the Department of Licensing website and contains all electric vehicles
registered in the state of Washington. By randomly sampling 5,000 of the 109,000 electric vehicles registered, I have created a sample representative
of the entire dataset and formed it into an interactive experience to explore the electric vehicles' makes, ranges, and locations.

In this interactive dashboard, the heatmap graph on the left displays the number of electric vehicles registered in each Washington State city seperated
by their electric range. The bar graph on the right displays the number of each make of electric vehicle seperated by the type of electric vehicle.
By dragging and selecting areas on the heatmap graph, the electric vehicle records used to generate the bar graph are updated.

<vegachart schema-url="{{ site.baseurl }}/assets/json/Final_dashboard.json" style="width: 100%"></vegachart>

Although the sample used to generate these graphs are only 5,000 of the 109,000 records from the dataset, the random selection of records
maintains the ratios of the data, meaning the sample is an accurate representation of the full dataset. The full number of records in each catagory
can be extrapolated by multiplying the values by ~21 times.

Another main concern for people interested in buying or supporting the development of electric vehicles is how environmentally sustainable, or 'green',
 they are. The visualization below displays the amount of Clean Alternative Fuel Vehicle (CAFV) eligible vehicles in each Washington State city. It also
 shows the amount of unknown and ineligible vehicles in each city.

<vegachart schema-url="{{ site.baseurl }}/assets/json/CAFV_eligibility.json" style="width: 100%"></vegachart>

Washington, however, is not the only state on the forefront of electric vehicle production and regristrations. In order to provide some context, this is a graph of
 electric vehicle range and efficiency across the U.S.

<iframe style="width: 900px; height: 633.537px;" src="https://afdc.energy.gov/data/widgets/10963" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"></iframe>

The overall amount of electric vehicles registered in the U.S. is increasing each year. States such as California, Washington, and Florida are
leading the way in producing and registering clean, electric vehicles. Below is a graph from the U.S. Department of Energy showing the registered
electric vehicles in 2022 by state.

<iframe style="width: 900px; height: 619.075px;" src="https://afdc.energy.gov/data/widgets/10962" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"></iframe>

Clean energy vehicles, specifically electric vehicles, are becoming more popular by the day. Serving as a complete alternative to gas-powered
 vehicles, these feats of engineering are revolutionizing the automobile industry and are providing another option for people who want to live a
 more sustainable life. Unfortunately, the capabilities of electric vehicles are not fully comparable to gas-powered vehicles yet. I hope this evaluation
 of Washington's registered electric vehicles helps to provide a realistic view of the current status of electric vehicles, their cleanliness, and their efficiency
 as they are now.

Works Cited:

Maps and data - average range and efficiency of U.S. Electric Vehicles. Alternative Fuels Data Center: Maps and Data - Average Range and Efficiency of U.S. Electric Vehicles. (n.d.). Retrieved December 2, 2022, from https://afdc.energy.gov/data/10963 

Maps and data - electric vehicle registrations by State. Alternative Fuels Data Center: Maps and Data - Electric Vehicle Registrations by State. (n.d.). Retrieved December 2, 2022, from https://afdc.energy.gov/data/10962 

Publisher data.wa.gov. (2022, November 18). Electric Vehicle Population Data. Catalog. Retrieved December 2, 2022, from https://catalog.data.gov/dataset/electric-vehicle-population-data 

<!-- these are written in a combo of html and liquid --> 

I've tried and tried and for some reason the button links below are stuck leading to the wrong analysis and data. The correct links are:

Data: https://github.com/AshtonJA/AshtonJA.github.io/blob/main/_data/Electric_Vehicle_Population_Data.csv

Analysis: https://github.com/AshtonJA/AshtonJA.github.io/blob/main/python_notebooks/Anaya-Ashton-FinalProject1.ipynb

<div class="left">
{% include elements/button.html link="https://github.com/AshtonJA/AshtonJA.github.io/blob/main/_data/Electric_Vehicle_Population_Data.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/AshtonJA/AshtonJA.github.io/blob/main/python_notebooks/Anaya-Ashton-FinalProject1.ipynb" text="The Analysis" %}
</div>

