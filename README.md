# Covid_19-Analysis
Our project is helpful in visualizing several differences brought about at industrial, climatic and
public level due to the pandemic by comparing historical data (before 2020) to that of the years 2020-
21. We also plan to implement machine learning module to interpret post pandemic stock prices and
performance of different industries based on the current data.
  1: Requirement Analysis
1. Visualization Modules:
• Streamlit
• Matplotlib
• Plotly
• Folium
.
2. Data Reading and Storage Modules:
• Pandas
• Pandas Data Reader
• MS Excel
3. Computation Modules:
• NumPy
• DateTime
• SK-learn
• Tensorflow
All the above modules are required by the end user to implement the project on their machine.
2 Solution Methodology:
Modules included are:
• Climate Screen.
• Economy Screen.
• Public Health Screen.
Climate Screen:
Data used is static and is read into a Pandas data-frame.
• For the first graph, the data is segregated into 6 data frames of 6 different cities. Then the AQI indices are given as parameters to the plot function which are selected from a drop-down list in the Streamlit app.
• For the second graph, the data is cleaned using dropna and fillna functions, segregated into different time intervals(2019 and 2020) and visualized in the form a comparison bar chart.
Economy Screen:
• For the first graph the data is segregated into 4 time intervals (2017,18,19,20), then it is grouped sector wise and a mean annual turnover is calculated using the NumPy mean function.
• For the second graph the same procedure is followed except here the data is grouped company wise for the years 2019 and 2020 which was earlier segregated.
• In the third graph NIFTY and BSE index data is gathered from yahoo finance and plotted using matplotlib methods.
• The last graph’s data is gathered from worldbank.org and the unemployment rates are plotted in the form on of line graph.
Public Health Screen:
• For all the plots, the data is collected from the GitHub repository of John Hopkins University.
• In the first plot, data is read into a data frame and cleaned then only the top 6 countries affected by covid-19 are selected using numerical analysis and then a scatter chart is plotted
• In the second plot, the option to type a country’s name in the app is given as a parameter to the plot function which displays given country’s graph.
• For third, fourth and the final heat map the same data frame is used just in the form of bar charts for the former and a world map (folium) for the latter.
