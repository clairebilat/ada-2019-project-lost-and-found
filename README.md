# Where to eat in Chigago : an analysis of the inspections from the Chicago department of Public Health's Food Protection Programm

# Abstract
The Chicago department of Public Health’s Food Protection Program provides a database which contains information from inspections reports of restaurants and other food establishments in Chicago from 2010 to nowadays. It contains many information about the establishments, like the type of facility (groceries’ stores, restaurants, coffee shop, …), and their locations. Many information about the violations detected are also provided in the database, like the reason that led to the inspection.

In our project we endeavor to visualize the healthiness of public food establishments according to the type of facility, their ward and the date of the inspection. An analysis of the violation’s type according to these three parameters will also be conducted. The principal questions we'll answer are : which ward of Chicago are the most healthy and unhealthy ? Which type of facility tend to be more unhealthy ? Did the healthiness of the food in Chicago increase or decrease from 2010 until now ?
Others questions can appear during the analysis and be add to these.

The purpose of the project is to help the consumer to easily choose where to eat in Chicago, but also to help the Chicago department of Public Health’s Food Protection Program to adapt their response and work (for example, where should a prevention program be proposed).

# Research questions
 
- How to take the appropriate precautions when viewing or analyzing these data in order to manage the duplicatas ?

- Which facilities' types will we focus on ?

- How to deal with establishments that were inspected multiple times (for example in 2010 and in 2013) in a general view ?

- How to take into account the esthablishments with multiple violations ?

- How to manage the fact that the violations' definitions have changed in 2018 ?

- How will the healthiness of an establishment be implemented ?

- How to implement a good vizualisation tool (an interactive map for example) ?


# Dataset

The dataset that will be used is the Chicago Food Inspection from the list provided. 
Focusing on the rows, we will have to take care of the duplicatas.
We'll have to process the violation's column in order to only take the id of the different violations (not the comments).
As the violations' definition has changed in 2018, we will have to find a way to consider and manage this change. It has been specified that two datasets exist, one for the datas before 2018 and one for the datas after; either we will focus our attention on one of the two or we will have to find a way to merge them.
We'll need to add a new column calculating the healthiness of an establishment (the method to calculate this healthiness is not yet defined).

# A list of internal milestones up until project milestone 2
 
 - (1st week) Clean the dataset : manage the duplicatas, the multiple occurences for an establishment due to multiple inspections, clean the violation column 

- (2nd week) Take a look at the dataset in order to have an idea of the data's distribution :
    - which are the most represented establishments ? Which ones will we study ?
    - what are the most common violations ?
    - how will we implement the healthiness of an establishment ? Take only the risk factor into account or also the type of violation ? If so, how to classify them ?
    - Are the locations well distributed or is a ward-study irrelevant ?
    
- (3rd week) Answer the questions (healthiness of public food establishments according to type facility, ward and time ; violation's type according to facility's type, ward and time). Identifiy if other questions are interesting to answer.

- (4th week) Create the interactive map (if it's still meaningfull) and the visualization.


# Questions for TAa
Does our project seem reasonable and interesting enough for the purpose of the exercise and which questions seem most promising (to know what to focus on first) ?

