---
layout: post
title:  "Let's see the data"
author: JD Gardner
description: How can we see the data we are going to analyze.   
image: "/assets/images/cover.jpg"
---

# _What is data visualization?_
Data visualization is putting the data into a non numeric form so that we have a picture to see the trends of the data. We often use graphs to accomplish this. In the world of statistics we refer to graphs as plots in data visualization. There are different plots that show us different aspects of our data. [geekforgeek](https://www.geeksforgeeks.org/data-visualization-and-its-importance/)
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
There are 4 libraries that are used to help us in our data visualization:
- matplotlib
- seaborn
- plotly
- bokeh
The one that is most commonly used in python data visualization is the matplotlib library. This package allows the use of basic visualization methods such as: line plots, scatter plots, box plots, etc. The seaborn package is useful for heatmaps, which are not used as much in the beginning exploratory data analyses. Plotly has interactive plots that allow us to see the difference in data as we change it. Similar to plotly, the bokeh package is also interactive but more for web applications.

## _How we use the packages_
For each library we have to install the library before we use its functions. Each library has a unique call to create the different plot that we want(in the next section see some examples).

## _Examples_
example of plotting data using a scatterplot in matplotlib
```python
import matplotlib.pyplot as plt
x = [1, 2, 3, 4, 5]
y = [10, 20, 25, 30, 35]
plt.scatter(x, y, color='blue', marker='o')
plt.title('Sample Scatter Plot')
plt.xlabel('X-axis Label')
plt.ylabel('Y-axis Label')
plt.show()
```
![Scatter Plot](assets/images/scatterplot.png)
[scatter plot](https://www.datascienceblog.net/post/data-visualization/scatterplot/)
```python
import seaborn as sns
import matplotlib.pyplot as plt
data = {
    'category': ['A', 'A', 'A', 'B', 'B', 'B'],
    'value': [10, 20, 25, 30, 35, 40]
}
import pandas as pd
df = pd.DataFrame(data)
sns.boxplot(x='category', y='value', data=df)
plt.title('Sample Box Plot')
plt.xlabel('Category')
plt.ylabel('Value')
plt.show()
```
![Box Plot](assets/images/boxplot.jpg)
[boxplot](https://discovery.cs.illinois.edu/learn/Exploratory-Data-Analysis/Quartiles-and-Box-Plots/)

```python
from bokeh.plotting import figure, show
from bokeh.io import output_notebook
from bokeh.transform import dodge
import numpy as np
output_notebook()
data = np.random.randn(1000)
p = figure(title="Sample Histogram", x_axis_label='Value', y_axis_label='Frequency')
hist, edges = np.histogram(data, bins=30)
p.quad(top=hist, bottom=0, left=edges[:-1], right=edges[1:], fill_color="navy", line_color="white", alpha=0.5)
show(p)
```
![Histogram](assets/images/histogram.jpg)
[histgram](https://docs.bokeh.org/en/0.8.2/docs/user_guide/charts.html)

```python
import seaborn as sns
import matplotlib.pyplot as plt
import numpy as np
data = np.random.rand(10, 12)
sns.heatmap(data, annot=True, cmap='coolwarm')
plt.title('Sample Heatmap')
plt.xlabel('X-axis Label')
plt.ylabel('Y-axis Label')
plt.show()
```
![Heatmap](assets/images/heatmap.jpg)
[heatmap](https://indianaiproduction.com/seaborn-heatmap/)
## _Try it for yourself_
Try plotting some data for yourself! in my example you can see that I just created a sample data set. You can copy this and run it on your own computer to see what it produces and how it can help you visualize your data in your next project. 