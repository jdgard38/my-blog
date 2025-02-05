---
layout: post
title:  "Let's see the data"
author: JD Gardner
description: How can we see the data we are going to analyze.   
image: "/assets/images/image5.jpg"
---

# _What is data visualization?_
Data visualization is putting the data into a non numeric form so that we have a picture to see the trends of the data. We often use graphs to accomplish this. In the world of statistics we refer to graphs as plots in data visualization. There are different plots that show us different aspects of our data.
## _Plots_
Types of plots commonly used in analytics:
- Scatter Plot
- Box Plot
- Histogram
- Bar Chart
- Heatmap

Scatter plots are useful in helping us see the relationship between two variables. 
Box plots are helpful in showing us where the median, quartiles, and outliers lie, while showing us the distribution of the dataset.
Histograms are mostly helpful in showing the distribution of the data.
Bar charts are good for comparing categorical data.
Heatmaps show us data information in more ways than just lines, often using color to respresent the data in matrix formats.

## _Packages/libraries needed_
what packages are needed to plot data in python
matlibplot
seaborn
plotly
bokeh
## _How we use the packages_
how do we use those plots
## _examples_
- example of plotting data using a scatterplot
---
import matplotlib.pyplot as plt
x = [1, 2, 3, 4, 5]
y = [10, 20, 25, 30, 35]
plt.scatter(x, y, color='blue', marker='o')
plt.title('Sample Scatter Plot')
plt.xlabel('X-axis Label')
plt.ylabel('Y-axis Label')
plt.show()
---
give examples of plots and code