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
We obtained our dataset through the following link: https://catalog.data.gov/dataset/nypd-arrest-data-year-to-date. The dataset, "NYPD Arrest Data (Year to Date)", contains information about arrests made by the New York City Police Department. It comprises 63,621 entries, each representing an individual arrest record, distributed across 19 different columns that provide various details about each arrest.

Here is a breakdown of the columns and the types of data they contain:

1. **ARREST_KEY**: A unique identifier for each arrest (integer).
2. **ARREST_DATE**: The date on which the arrest was made (string, formatted as date).
3. **PD_CD** (Police Department Code): A numerical code representing the specific charge of the arrest (float).
4. **PD_DESC** (Police Department Description): A description of the charge (string).
5. **KY_CD** (Key Code): A numerical code categorizing the offense (float).
6. **OFNS_DESC** (Offense Description): A description of the offense category (string).
7. **LAW_CODE**: The specific law or statute under which the arrest was made (string).
8. **LAW_CAT_CD** (Law Category Code): The severity of the offense (e.g., felony, misdemeanor) (string).
9. **ARREST_BORO**: The borough in which the arrest occurred, denoted by a single letter (string).
10. **ARREST_PRECINCT**: The precinct number where the arrest occurred (integer).
11. **JURISDICTION_CODE**: A code indicating the jurisdiction responsible for the arrest (integer).
12. **AGE_GROUP**: Categorical age range of the arrestee (string).
13. **PERP_SEX**: Gender of the person arrested (string).
14. **PERP_RACE**: Race of the person arrested (string).
15. **X_COORD_CD** and **Y_COORD_CD**: Cartesian coordinates for mapping the event in the New York State Plane Coordinate System (integer).
16. **Latitude** and **Longitude**: Geographic coordinates of the arrest location (float).
17. **New Georeferenced Column**: A textual representation of the geographic location in a "POINT (longitude latitude)" format (string).

The dataset contains a mix of numeric and categorical data, providing a comprehensive view of the circumstances surrounding each arrest, including demographic data about the arrestees and specific details of the legal charges against them. This data can be used for statistical analysis to identify trends, assess law enforcement activity, and understand crime patterns in New York City.

## Research Questions

### Question #1: 
  What is the distribution of arrests across different boroughs of New York City for the age groups of <18 and 18-44, and what insights does this distribution provide into law enforcement practices, social demographics, and potential disparities?

#### Importance:
  The data obtained from this question can inform policymakers about the effectiveness and impact of law enforcement strategies. If there are significant differences in arrest rates among boroughs or age groups, it could prompt the need for policy changes or interventions to address underlying issues.

### Question #2: 
  What is the annual trend and distribution of robbery-related arrests throughout the year, and how do variations in arrest rates provide insights into patterns of criminal activity, law enforcement efforts, and potential factors influencing robbery incidents?

#### Importance:
  By examining the annual trend and distribution of robbery-related arrests, especially in correlation with retail sales data, researchers can discern if there are seasonal patterns in criminal activity. This can shed light on whether certain times of the year, such as the holiday season with higher retail sales, coincide with an increase in robbery incidents.


## Manipulations and Calculations

### Question #1: 
While we did not have to manipulate or alter the initial data set in order to make our visualization presentable and useful, we did have to make slight alterations to data types in order to successfully build our first visualization. First, we had to change the latitude and longitude data pills in Tableau to continuous dimension data types. At first, these pills were continuous data pills that were being mapped based on their average latitude and longitude, which would not have allowed us to sufficiently map crime across New York City’s five boroughs. Next, we filtered the age groups to only show the distribution of arrests involving 18-44-year-olds across New York City, as opposed to <18 to 65 and older. We added this filter in an effort to ensure that the visualization did not include too much data, thereby making it difficult to read and interpret. Lastly, we differentiated the different boroughs of New York City according to color, while also adding large circles onto the areas of the city where the highest concentration of arrests were made. 

### Question #2:
While we did not have to manipulate the initial data set in order to make our visualization useful, we did make slight alterations to the data in the creation of the above line graph. First, because we decided to create a visualization showing trends of only robbery-related arrests, we had to filter the data so as to only show arrest data for arrests whose offense descriptions were robbery related. These offenses included “robbery,” “burglary,” “burglar’s tools,” “possession of stolen property” and any type of “larceny” and “theft”. Next, we had to change the “arrest key” data pill from discrete to a continuous dimension. This allowed us to count the number of arrests per offense and subsequently map the resulting data on the line chart. Lastly, we filtered the offense descriptions by color on the line chart while also adding a forecast for the five months following the completion of data collection for the data set. 
## Analysis and Results

### Question #1: 
The more densely populated areas have more arrests as expected. The disparities in lower population areas arrests compared to more highly populated areas suggest that due to there being more easy anonymity in largely populated parts of New York, crime increases. This chart also allows policymakers to see the areas where more enhanced police presence is needed. For example, most of Staten Island doesn't have much crime except for the northeasternmost part of it so more police is likely needed there. In the line chart, it can be seen that the summer months, especially June, have higher arrests among the younger age group. This likely is because they no longer have school to occupy them and a solution to this is for there to be more, affordable activities for the youth to participate in when school is out. Finally, black and hispanic people are the most arrested demographics by far. This is likely due to the higher poverty rates associated with them and the fact that they feel like crime is the only way out of poverty.

### Question #2: 
As we see in the graph there is some fluctuation in the arrests throughout the year. These might be for seasonal variation. There is a noticeable increase from January to May. These months may present more opportunities for robbers as post holiday periods often mean homes are stocked with valuable items. Robbery related offenses tend to decrease during the summer months, possibly because people are often away on vacation, leaving their valuables in secure locations away from home. Other external factors that may influence high rates of robbery related offenses are the economic state. The economic state of New York City in the beginning and end of 2023 might have been declining, potentially increasing the rate of robbery related crimes. This would be understandable because periods of economic decline may result in higher unemployment rates and financial desperation which can motivate people to commit robbery related crimes. We were able to forecast our findings for the next 5 months and we see an overall gradual increase in the trend. This makes sense because as the population and economy grow, there is typically an uptick in the occurrences of robberies.

## Tableau Packaged Workbook
