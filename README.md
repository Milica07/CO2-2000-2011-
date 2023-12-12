# CO2-2000-2011-
Through this repository I will share my project correlated to data visualization (Tableau)
In this project different data sources are linked in Tableau and multiple datasets are visualized (comparisons and combinations of data).

Attached files in Tableau are: CO2 Dataset, Energy data, gdptotal, totalpopulation

##### Making and visualizing JOINs in Tableau 
###### The scenario
I am working as a data analyst at a policy research institute. For my current project, I need to create a visualization that shows the CO2 emissions per capita for each country from 2000-2011. I need to provide a visual presentation that not only allows someone to visually compare CO2 emissions between countries from year to year, but also provides information about each country's population, GDP, and energy use.
I already have a dataset that includes emissions for each country between the yaers 1960-2011. But, the information that I need on energy use, total population, and GDP I had to collect from a government website. Each dataset is in a separate file. Moreover, some of the information is missing for some countries. But, in this case the missing information is from the 1960s, 1970s, and 1980s.
My project is only concerned with the data from 2000-2011. I need an efficient way to utilize some data from one source, and some data from other sources. Tableau allows linking data from different sources, as well as import data from different formats. In this assignment I won't be working with one data source and I will use a Web Data Connector. This tool allows me to import the data directly from another site. My visualizations will update when the data sources for my visualization are updated. 

###### Load the data
I loaded all datasets in Tableau Public.

###### Make connections with JOINs
Setting up the connections between the different datasets by creating JOINs between them. 
Double-click on CO2 dataset, double-click on CO2 Data Cleaned.
On the CO2 Data Cleaned box click on the arrow and select Open.

Click on the Energy dataset under Connections.
Drag the energy sheet across to the CO2 Data Cleaned box under Multiple Connections. A pop-up window for a Join will appear.
I made Inner Join between Year and Country name columns. (CO2 Data Cleaned & Energy)
Since Year and Year1 had a number sign above them I have changed the data type to Date for each of these columns. 
Year(Gdptotal) as well needed to change.
I made Inner Join between Year and Country name columns (Energy & gdptotal).
Year(totalpopulation) column as well needed to change data type to Date.
I made Inner Join between Year and Country name columns (gdptotal & totalpopulation).
Click Update Now to view data columns.
The only years in the dataset are between 2000-2011. While dataset CO2 went from 1960-2011, and other datasets went from 2000-2015, the intersection only includes 2000-2011. That is the time span that I needed for this task.
Additional changes in data types: column Energy use and currentGDP changed to Number(decimal) and Number(whole).

###### Create a visualization
Open Sheet 1.
Country name draged into the Detail square.
CO2 Per Capita draged into the Color square.
The color was changed from Automatic to Red-Green diverging.
The boxes Stepped Color and Reversed was checked (because green is generally viewed as positive for CO2 emissions).
Click the Show Advanced dropdown, check the Start and End boxes (Start = 0; End = 62).
Drag Year from under CO2 Data Cleaned into the Filters area(Years, Next, All, OK). + Show filter
Click on the arrow to the right of YEAR(Year) on the far-right side of the screen and select Single Value(dropdown).
See attached PNG file: CO2 emissions per capita for each country for 2010






Link to the Tableau: [https://public.tableau.com/shared/77DPGSP29?:display_count=n&:origin=viz_share_link](https://public.tableau.com/shared/TTNG3CXTR?:display_count=n&:origin=viz_share_link)https://public.tableau.com/shared/TTNG3CXTR?:display_count=n&:origin=viz_share_link
OR
https://public.tableau.com/shared/DD4MXMC5W?:display_count=n&:origin=viz_share_link








