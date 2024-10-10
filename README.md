# The-Temporal-Spatial-Changes-of-Unemployment-Rate-in-Contiguous-USA

The temporal-spatial changes of unemployment rate in contiguous USA are a significant topic for data visualization because it can reveal the socio-economic conditions of different regions and states over time. It can show how they are impacted by several factors such as crime, incarceration and murder rates. The unemployment rate is a key indicator of labor market performance and economic progression, and it impacts income, poverty, health, education, and social stability. Previously it has been shown that unemployment rate varies across different regions and states in the US, and that it is influenced by factors like business cycles, demographic changes, industrial composition, labor mobility, and policy interventions. Moreover, unemployment may also impact other social outcomes, such as crime, incarceration, and murder rates. The magnitude of these relationships is not clear and may depend on various contextual and individual factors. Therefore, visualizing the temporal-spatial changes of unemployment rate in contiguous USA can help us understand and compare the socio-economic situations of different regions and states, and explore the potential associations and causalities between unemployment and other variables. 
 
Goals: 
•	Analyze the trends and cycles of unemployment rate at the national, state, and county levels over time in the US. 
•	Identify the states and regions with the highest and lowest unemployment rates. The spatial representation of the unemployment rate changes over time. 
•	Investigate the correlation of the unemployment rate and crime rate and how they vary across different states and regions. 
 
 
 
 
Data cleaning and processing: 
This project is done in R programming language. For this project we will be aiming at exploring the relationship between unemployment and crime rates across different U.S. states. We need to clean and process the data which will be used for further analysis or visualization. The datasets used for this project are:  
Unemployrate: This dataset contains the monthly data on unemployment rate for each county in the US from 2007 to 2018. This data can be used to analyze the temporal and spatial patterns of unemployment rate in the US at the county level, and to see how unemployment rate differs across different counties and states, and over time. 
Crimerate: This dataset contains the annual data on violent crime rate, property crime rate, and incarceration rate for each state in the US from 2001 to 2016. This data can be used to analyze the relationship between unemployment rate and crime rate and to see how these variables vary across different states and over time. 
 
Murder Rates, States by region: This file contains the annual data on murder rate for each state in the US from 1987 to 2020, as well as the region and division classification for each state.  
 
Data cleaning and processing includes transforming raw data into a more usable format for analysis. This includes tasks such as removing or handling missing values, filtering relevant data, aggregating data, renaming columns, and creating new variables based on existing ones.  In this project first we filtered out non-contiguous states from the States and Unemployrate datasets. Then Aggregated the Unemployrate data by state and year, calculating total labor force, total employment, total unemployment, and mean unemployment rate. After that renamed the State column to STUSPS in Unemployrate which filtered the data for years 2007 to 2014. Similarly, renamed columns in Crimerate, filtered out non-contiguous states and the federal jurisdiction, and also filtered for years 2007 to 2014. Finally, we transformed state names to their abbreviations and calculated a new Crimerate column as the total violent crime per 100,000 population. It also rounds all numeric columns to 1 decimal place. 
 
 
Plotting The Graphs: 
 
Several plotting methods were utilized such as ggplot2 and plotly to illustrate the parameters throughout the process. The graphs we have used for visualizing the information are: 
 
•	Two time series visualizations using line plots to show the unemployment rate changes along with years and the crime rate changes along with years.  
•	A spatial map over the contiguous USA for the unemployment rate and crime rate for a specific year 
•	A scatter plot showing the relationship between unemployment rate and crime rate for a 
specific year. 
 
 
1.	Time Series Plots: Creates time series line plots for both unemployment rates and crime rates using the plotly library. 
  
 ![image](https://github.com/user-attachments/assets/bd386c90-e04a-435a-91b9-12ae7514d7db)


![image](https://github.com/user-attachments/assets/9ee032af-bb67-4d0c-ad0c-0e4f4f4b4c94)

  
2.	Data Filtering for 2014: Filters the Unemployrate and Crimerate datasets for the year 2014. 
3.	Data Joining: Joins the Unemployrate_2014 and Crimerate_2014 datasets on the State and Year columns. 
4.	Scatter Plot: Creates a scatter plot showing the relationship between unemployment rate and crime rate in 2014. 
 
 ![image](https://github.com/user-attachments/assets/0e21baa6-1891-469b-a24f-c62a7f1c542d)

             
5.	Spatial Plots: Joins the Contiguous_state and Unemployrate_2014 datasets and creates a spatial plot showing the unemployment rate in 2014. Similarly, joins the 
Contiguous_state and Crimerate_2014 datasets, and creates a spatial plot showing the crime rate in 2014. 
 
 
 ![image](https://github.com/user-attachments/assets/7f66f38e-cf01-4268-b4da-f53ca6db2dab)
 
 ![image](https://github.com/user-attachments/assets/9e96b7d5-132e-4587-98c6-22ff74140c31)

 
 
 
  
Results/Findings: 
The Relationships between X and Y: 
The analysis of the datasets reveals a complex relationship between the unemployment rate (X) and crime rate (Y) in the interactive scatter plot for the year of 2014. The trends and cycles of these variables at the state level over time in the US show a significant correlation. However, the strength and direction of this correlation vary across different states and regions. 
The Significance of Differences Among X and Y: 
The differences between the unemployment rate and crime rate are statistically significant from the interval of 2007 to 2014. The unemployment rate was at its peak in California in the year 2010. The crimerate was at its peak in the year 2007 in California. The states and regions with the highest and lowest unemployment rates also show distinct patterns in their crime rates. These differences suggest that the socio-economic conditions and policy interventions in these states and regions significantly impact unemployment and crime rates. 
The Temporal and Spatial Changes of Variables X and Y: 
The temporal-spatial changes of the unemployment rate and crime rate in contiguous USA are visualized through time series plots and spatial plots. These visualizations show how these variables have changed over time and across different states and regions. They reveal the patterns, trends, differences, and relationships of these variables, and support the claims and conclusions based on the data. 
 
 
 
Discussion: 
This project's findings are consistent with the goals showing a correlation between unemployment and crime rates. The business cycles, demographic changes, industrial composition, labor mobility, and policy interventions in different states and regions can influence both unemployment and crime rates. Moreover, the unemployment rate can impact other social outcomes, such as income, poverty, health, education, and social stability, which in turn can affect the crime rate. 
The implementation of this project involves data cleaning, transformation, and visualization using R and several libraries. The pros of this approach include the flexibility and power of R for data analysis and visualization, and the richness and diversity of the datasets used. The cons include the complexity and time-consuming nature of data cleaning and transformation, and the potential issues with data quality and consistency. The current data visualization effectively conveys the temporal-spatial changes of unemployment rate in contiguous USA, but it could be improved by incorporating more interactive and dynamic features to plot the spatial graphs, and by addressing the potential issues with readability and informativeness. 
 
 
HTML File: 
file:///C:/Users/salsa/OneDrive/Desktop/MS-
DS/Data%20Visualization/Final%20Project/Final%20Project%20Codes/Final_Project_Code.ht ml 
