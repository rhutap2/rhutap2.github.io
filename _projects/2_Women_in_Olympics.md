---
name: Women in Olympics
tools: [Python, HTML, vega-lite]
image: assets/pngs/Olympics-Logo-2010-present.png
description: A short analysis on womens participation in Olympics by Rhuta Patki
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Women in Olympics

## Introduction:

Gender and racial inequality has been a major issue in societies around the golbe. Numerous efforts have been made to allow people equal opportunities regardless of who they are or where they come from. Sport has been a powerful platform for conveying social messages to the masses. This project aim to study womens participation in the Olympic Games. 

<br>Our datasets: <br/>
1. Primary Dataset: <br>
[120 years of Olympic history: athletes and results](https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results?resource=download): This dataset was sourced from 'Kaggle'. It contains data about the atheletes who participated such as their name, sex, age, height, weight, the team they belonged to, the Olympic year and season (Summer, Winter), city where the games were hosted, the sport, event and any medals they won, etc.

2. Contextual Dataset:<br>
[Women in the Olympics](https://data.world/sports/women-in-the-olympic-games): This dataset was sourced from 'data.world' and was initially published as a part of the 'Women in the Olympic Movement' factsheet on the [Official website of the Olympics](https://olympics.com/en/). This dataset contains a record of the Olympics women's sports and the year they were introduced in as well as statistical data about the women participants over the years.


## Dashboard:

<vegachart schema-url="{{ site.baseurl }}/assets/json/main_dashboard.json" style="width: 50%"></vegachart>
<br>
The dashboard above contains 3 charts. The first chart shows us the total matches of a sport played by a team. The teams have been represented by the National Olympic Committee (NOC) they belong to (National Olympic comities are represented by a 3-letter code also referred to as the 'NOC'). Simply hovering over a block in the chart will tell you the number of games played of a particular sport by a particular team. Clicking on the block with update the 2 charts on the bottom to show data about the sport and the country that was selected. The charts on the bottom show the year when a particular country's Men's and Women's team's first participated in the a sport. For most sports played by most countries, the Men's team played the sport long before the Women's team did.<br>
(Note that the Y-axis here does not start from 0. This is to enunciate the year gap between the two genders.)<br>
<br>




## Participation of Women in Olympics over time:
<br>
The below visualizations present the data published in the 'Women in the Olympic Movement' factsheet by the International Olympic Committee. 

#### Percentage of Women's events over time:<br>
<vegachart schema-url="{{ site.baseurl }}/assets/json/chart1.json" style="width: 100%"></vegachart>
<br>
To encourage women's participation in international sports and provide them with equal opportunities as their male counterparts, the International Olympic Committee has been committed to progressively introduce new sports in the Women's category. Women's Olympic games were first introduced in 1900. [Of a total of 997 athletes, 22 women competed in five sports: tennis, sailing, croquet, equestrianism and golf.](https://olympics.com/ioc/faq/history-and-origin-of-the-games/when-did-women-first-compete-in-the-olympic-games#:~:text=Women%20competed%20for%20the%20first,to%20gender%20equality%20in%20sport)
Today there are roughly 50 Olympic sports that women can participate in.
<br>
<br>

#### Women's Olympic participation in 1900 vs. 2016:<br>
<vegachart schema-url="{{ site.baseurl }}/assets/json/pie_charts.json" style="width: 100%"></vegachart>
<br>
Efforts taken by the International Olympic Committee have largely changed women's involment in the Olympic games. As of 2016, women constitute about 45% of the total participants as against a mere 2.2% when it first started in 1900.
<br>

<br>
Project References:<br>
[1] https://data.world/sports/women-in-the-olympic-games <br>
[2] https://www.kaggle.com/datasets/heesoo37/120-years-of-olympic-history-athletes-and-results?resource=download <br>
[3] https://olympics.com/ioc/faq/history-and-origin-of-the-games/when-did-women-first-compete-in-the-olympic-games#:~:text=Women%20competed%20for%20the%20first,to%20gender%20equality%20in%20sport.<br>
[4] https://olympics.com/ioc/gender-equality/gender-equality-through-time/at-the-olympic-games<br>



## Search The Data & Methods


<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/building_inventory.csv" text="The Data" %}
</div>


<div class="right">
{% include elements/button.html link="https://github.com/jnaiman/online_cv_public/blob/main/python_notebooks/test_generate_plots.ipynb" text="The Analysis" %}
</div>

