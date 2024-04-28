# MIST4610-Group-Project-2

## Team Name: 
21484 Group 5 

## Team Members:

1. Grace Conn [@graceconn](https://www.github.com/graceconn)
2. Rhea Sabat [@rheasabat](https://www.github.com/rheasabat)
3. Bryce James [@brycejam](https://www.github.com/brycejam)
4. Adam LeBrun [@adam4l](https://www.github.com/adam4l)
5. Josh Horwitz [@Josh-Horwitz-1219](https://www.github.com/Josh-Horwitz-1219)

## Dataset Description
The "NYPD Arrest Data (Year to Date)" dataset encapsulates a comprehensive snapshot of arrests made in New York City, meticulously chronicled across 63,621 entries and 19 distinct columns. This dataset is publicly accessible via the NYPD's data portal, ensuring transparency and facilitating a deeper understanding of crime trends within the city. The dataset incorporates a mix of data types to represent a variety of dimensions related to each arrest event. Key identifiers such as `ARREST_KEY` and `ARREST_DATE` are presented as strings, capturing the unique ID of each arrest and the date on which it occurred, respectively. Detailed descriptions of offenses are also string data types, including `PD_DESC` (police department descriptions) and `OFNS_DESC` (offense descriptions), along with `LAW_CODE`, which details the specific legal statutes violated. Administrative data such as the borough (`ARREST_BORO`), precinct (`ARREST_PRECINCT`), and jurisdiction code (`JURISDICTION_CODE`) of the arrest are included as strings. Demographic information about the perpetrators, such as age (`AGE_GROUP`), sex (`PERP_SEX`), and race (`PERP_RACE`), is also recorded in string format. Geographic data, including coordinates (`X_COORD_CD`, `Y_COORD_CD`, `Latitude`, `Longitude`) and a geospatial representation of the location (`New Georeferenced Column`), are provided in number formats (whole for coordinates and decimal for geographical coordinates). This dataset not only serves as a resource for understanding the specifics of each arrest but also aids in analyzing broader crime patterns and demographics across New York City's diverse communities.

## Research Questions

### Question #1: 
  What is the distribution of arrests across different boroughs of New York City for the age groups of <18 and 18-44, and what insights does this distribution provide into law enforcement practices, social demographics, and potential disparities?

#### Importance:
  The data obtained from this question can inform policymakers about the effectiveness and impact of law enforcement strategies. If there are significant differences in arrest rates among boroughs or age groups, it could prompt the need for policy changes or interventions to address underlying issues. Additionally, disparities in arrest rates across boroughs and age groups can unveil systemic biases or inequalities within the criminal justice system. Persistent disparities may indicate issues such as racial profiling, socioeconomic inequalities, or differential treatment by law enforcement agencies. By scrutinizing these disparities, policymakers can identify areas for reform and implement measures to ensure fair and equitable law enforcement practices. 

### Question #2: 
  What is the annual trend and distribution of robbery-related arrests throughout the year, and how do variations in arrest rates provide insights into patterns of criminal activity, law enforcement efforts, and potential factors influencing robbery incidents?

#### Importance:
  By examining the annual trend and distribution of robbery-related arrests, especially in correlation with retail sales data, researchers can discern if there are seasonal patterns in criminal activity. This can shed light on whether certain times of the year, such as the holiday season with higher retail sales, coincide with an increase in robbery incidents. Also by examining the distribution of robbery-related arrests across different regions and time periods, it helps identify hotspots of criminal activity and emerging trends. By pinpointing areas with high concentrations of robbery incidents, law enforcement agencies can prioritize resources for targeted interventions, such as increased patrols, surveillance, or community outreach programs. Additionally, identifying trends in robbery tactics or target locations informs the development of proactive strategies to deter and apprehend offenders.


## Manipulations and Calculations

### Question #1: 
  While we did not have to manipulate or alter the initial data set in order to make our visualization presentable and useful, we did have to make slight alterations to data types in order to successfully build our first visualization. First, we had to change the latitude and longitude data pills in Tableau to continuous dimension data types. At first, these pills were continuous data pills that were being mapped based on their average latitude and longitude, which would not have allowed us to sufficiently map crime across New York City’s five boroughs. Next, we filtered the age groups to only show the distribution of arrests involving 18-44-year-olds across New York City, as opposed to <18 to 65 and older. We added this filter in an effort to ensure that the visualization did not include too much data, thereby making it difficult to read and interpret. Lastly, we differentiated the different boroughs of New York City according to color, while also adding large circles onto the areas of the city where the highest concentration of arrests were made. 

### Question #2:
  While we did not have to manipulate the initial data set in order to make our visualization useful, we did make slight alterations to the data in the creation of the above line graph. First, because we decided to create a visualization showing trends of only robbery-related arrests, we had to filter the data so as to only show arrest data for arrests whose offense descriptions were robbery-related. These offenses included “robbery,” “burglary,” “burglar’s tools,” “possession of stolen property” and any type of “larceny” and “theft”. Next, we had to change the “arrest key” data pill from a discrete to a continuous dimension. This allowed us to count the number of arrests per offense and subsequently map the resulting data on the line chart. Lastly, we filtered the offense descriptions by color on the line chart while also adding a forecast for the five months following the completion of data collection for the data set. 
## Analysis and Results

### Question #1: 

<img width="1054" alt="Screenshot 2024-04-28 at 4 41 51 PM" src="https://github.com/adam4l/MIST4610-Group-Project-2/assets/163042495/96bb8c4e-03a1-4aaa-a216-cadda60f41e3">

  The more densely populated areas have more arrests as expected. The disparities in lower population areas arrests compared to more highly populated areas suggest that due to there being more easy anonymity in largely populated parts of New York, crime increases. This chart also allows policymakers to see the areas where more enhanced police presence is needed. For example, most of Staten Island doesn't have much crime except for the northeasternmost part of it so more police is likely needed there. In the line chart, it can be seen that the summer months, especially June, have higher arrests among the younger age group. This likely is because they no longer have school to occupy them and a solution to this is for there to be more, affordable activities for the youth to participate in when school is out. Finally, black and hispanic people are the most arrested demographics by far. This is likely due to the higher poverty rates associated with them and the fact that they feel like crime is the only way out of poverty.

### Question #2: 

<img width="1062" alt="Screenshot 2024-04-28 at 4 42 17 PM" src="https://github.com/adam4l/MIST4610-Group-Project-2/assets/163042495/6bf787fb-30a2-4c58-98b4-dd93f1a81c81">

  As we see in the graph there is some fluctuation in the arrests throughout the year. These might be for seasonal variation. There is a noticeable increase from January to May. These months may present more opportunities for robbers as post-holiday periods often mean homes are stocked with valuable items. Robbery-related offenses tend to decrease during the summer months, possibly because people are often away on vacation, leaving their valuables in secure locations away from home. Other external factors that may influence high rates of robbery-related offenses are the economic state. The economic state of New York City at the beginning and end of 2023 might have been declining, potentially increasing the rate of robbery-related crimes. This would be understandable because periods of economic decline may result in higher unemployment rates and financial desperation which can motivate people to commit robbery-related crimes. We were able to forecast our findings for the next 5 months and we see an overall gradual increase in the trend. This makes sense because as the population and economy grow, there is typically an uptick in the occurrences of robberies.

## Tableau Packaged Workbook
The packaged workbook containing the visualizations shown above is attached to this repository.
