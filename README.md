# Where to eat in Chigago : an analysis of the inspections from the Chicago department of Public Health's Food Protection Programm

# Abstract
The Chicago department of Public Health’s Food Protection Program provides a database containing the information about inspections' reports of restaurants and other food establishments in Chicago from 2010 to the present. It contains many information about the establishments, like their type (groceries’ stores, restaurants, coffee shop, …) and their locations. There is also many information about the violations listed in the database, like their description and their causes and the reason that led to the inspection.

In our project we endeavor to visualize the healthiness of public food establishments according to their type of facility, their ward and the date of the inspection. An analysis of the violations’ types according to these three parameters will also be conducted. The impact of two other factors on the healthiness of food facilities in Chicago will be analyzed : first the correlation between the owner of an establishment and its healthiness will be studied ; we want to know if all establishements owned by an unhealthy owner are unhealthy or if those two factors are not correlated. Then we want to study the correlation between the healthiness of the establishments in Chicago and crime (according to the amount and gravity of crime in each ward).  

The purpose of the project is to help the consumer to easily choose where to eat in Chicago and to provide them an interactive and intuitive way to browse the different places offered to them. Also, it could help the Chicago department of Public Health’s Food Protection Program to adapt their methods relying on the situation described by the findings of the analysis (for example, if a prevention program should be proposed for a specific area or type of facility).

# Research questions
 
 The principal questions we'll answer are : 
 
    - Which wards of Chicago are the most healthy/unhealthy ? 
    - Which types of facilities tend to be less healthy ? 
    - Are the 'public' facilities (schools or hospitals) healthier than the 'privat' ones (restaurants) ?
    - Did the healthiness of the food in Chicago increase or decrease from 2010 until now ?
    - Do all establishments owned by the same person tend to have the same level of healthiness ?
    - Is the level of crime of an area correlated with the healthiness of the food in the same area ?

# Dataset

The first dataset that will be used is the Chicago Food Inspections from the list provided. 
Focusing on the rows, we took care of the duplicates. It involves managing the problem of the multiplicity of the inspections for a same establishment. 
We processed the violation's column in order to only take the id of the different violations (not the comments).
As the code has changed since 2010 (see http://dev.cityofchicago.org/open%20data/data%20portal/2018/06/29/food-violations-changes.html), we found a way to consider the changes and to manage what follows from it.
To get a general view of the healthiness of the establishments, we defined a function in order to quantify healthiness and added a new column expressing it of each establishment.

The second dataset will be Chicago Business Licenses and Owners (https://www.kaggle.com/chicago/chicago-business-licenses-and-owners).
With this database, we first needed to merge the two sub-databases : the license database, and the owner database.
For the owner database, we created a column with the full name (first + last).
We finally merged the two sub-set databases in one dataframe, and will merge this dataframe with the food-inspection one.

The third one will be the Crimes in Chicago database (https://www.kaggle.com/currie32/crimes-in-chicago).
For the rows, we had to take care of the duplicates. Some crimes may have been entered by two or more police officers, and thus created duplicates.
The principal information that interest us are the primary types of crimes, their latitudes and longitudes and the their community areas. The primary type column has been parsed to see if two types of crime are entered differently in the database (if two types of crime are the same but under different label). For the other columns, we had to deal with the missing values.
To compute the correlation between the level of crime and the healthiness score, we had to create a crime score. We used the minimum prison penalty for each type of crime and then compute this crimescore for each crime.

# A list of internal milestones up until project milestone 3 (report)
 
- (1st week) Start the analysis, and start answering the research questions :

    - Which wards of Chicago are the most healthy/unhealthy ? 
    - Which types of facilities tend to be less healthy ? 
    - Are the 'public' facilities (schools or hospitals) healthier than the 'privat' ones (restaurants) ?
    - Did the healthiness of the food in Chicago increase or decrease from 2010 until now ?
    - Do all establishments owned by the same person tend to have the same level of healthiness ?
    - Is the level of crime of an area correlated with the healthiness of the food in the same area ?
             
- (2nd week) See if we need to come back and process again our dataset according to our needs.
    
- (3rd week) Create the interactive map (if it's still meaningfull) and the visualization.

- (4th week) Finalize the analysis and the map, write the report or the data-story.

# Prospect

Analyzing other elements that can have an impact on the healthiness of food facilities in Chicago : the quality of life in different wards (or community area), the tourism repartition in Chicago,...


# Questions for TAs
Does our project seem still reasonable and interesting enough for the purpose of the exercise ?
