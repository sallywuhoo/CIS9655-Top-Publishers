# Analyzing Top Book Publishers

This is a group project I worked on for my CIS 9655 Data Visualization graduate course. My group and I decided to analyze top US book publishers and top US best selling novels; we split the work and my task was to create dynamic visualizations using the Vega-Altair visualization library on Python to showcase top publishers by awards and books that belonged to the top publishers.

To start, I initially had to manipulate the data on Excel; the origial CSV had all awards listed in 1 cell, but for the purposes of this analysis, each award needed to be in its own cell block so using Excel's built in functions, I separated out the awards. Next, I loaded this edited CSV file onto the Jupyter notebook and created a dataframe to hold the data; from there, I narrowed down the data to only include the necessary columns before creating the visualizations. In total, there were 1970 distinct publishing houses that have published award winning books in the file I was working with.

# Top Publishers
Using Altair, I created a dynamic bar graph that allows the user to hover the mouse over the bars to access further information such as the number of awards the publishing house published. For example, Penguin Random House has the tallest bar, and when the mouse is hovered over this bar, you can see they have 5491 awards. They're followed next by Harper Collins (1926 awards), then Macmillan (1795 awards), and then Simon & Schuster (1484 awards).

![top20publishers](https://github.com/sallywuhoo/CIS9655-Top-Publishers/assets/148400043/40f95d98-63ea-48ea-9bd2-a6e9082be3ad)

With these top 4 publishing houses, I created a sub-dataframe to hold only the data of these publishing houses to build the next visualization.

# Books Published by the Top 4 Publishing Houses
The second dynamic visualization I created shows a scatterplot on top with a bargraph below which are connected by the selection ability of the graph; this visualization allows users to point and drag their mouse over areas of the scatterplot to see which publishers have books within that enclosed space. On the scatterplot, each dot is represented by a book and the books' ratings are on the x-axis while its number of awards are on the y-axis; similarly, if you hover a mouse over the dot, additional information is provided such as the book title, its exact rating, and its exact number of awards. 
