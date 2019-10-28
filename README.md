# Where to eat in Chigago : an analysis of the inspections from the Chicago department of Public Health's Food Protection Programm

# Abstract
The Chicago department of Public Health’s Food Protection Program provides a database which contains the information from inspection reports of restaurants and other food establishments in Chicago from 2010 to the present. It contains many informations about the establishments, like their type of facility (groceries’ stores, restaurants, coffee shop, …) and their locations. Many informations about the violations listed are also provided in the database, like the description of the findings that caused them and the reason that invoked the staff from the program to led an inspection.

In our project we endeavor to visualize the healthiness of public food establishments according to their type of facility, their ward and the date of the inspection. An analysis of the violation’s types according to these three parameters will also be conducted. 

The principal questions we'll answer are : 
    - Which ward of Chicago are the most healthy and unhealthy ? 
    - Which type of facility tend to be more unhealthy ? 
    - Did the healthiness of the food in Chicago increase or decrease from 2010 until now ?

New problematics could be asked during the analysis and would be added to these.

The purpose of the project is to help the consumer to easily choose where to eat in Chicago and to provide them an interactive and intuitive way to browse the different places offered to them. Also, it could help the Chicago department of Public Health’s Food Protection Program to adapt their methods relying on the situation described by the findings of the analysis (for example, if a prevention program should be proposed for a specific area or type of facility).

# Research questions
 
- How to take the appropriate precautions when viewing or analyzing these data in order to manage the duplicates ?

- Which types of facility will we focus on ?

- How to manage the out of business or not located establishements ?

- How to deal with establishments that were inspected more than one time, and not necessarily for the same reason ?

- How to take into account the esthablishments with multiple violations ?

- How will the healthiness of an establishment be implemented ?

- How to get to a general view in order to compare the establishments effectively and wisely ?

- How to manage the fact that the Food Code Rules have changed since 2010 ?

- How to implement good vizualisation tools (an interactive map for example) ?


# Dataset

The dataset that will be used is the Chicago Food Inspections from the list provided. 
Focusing on the rows, we will have to take care of the duplicates. It involve to manage the problem of the multiplicity of the inspections for a same establishment.It is specified that establishments found to be out of business or not located are receiving a 'fail' of its inspection, this is an element to be careful about.
We'll have to process the violation's column in order to only take the id of the different violations (not the comments).
As the code has changed since 2010 (see http://dev.cityofchicago.org/open%20data/data%20portal/2018/06/29/food-violations-changes.html), we will have to find a way to consider the changes and to manage what follows from it. It has been specified that two datasets exist, one for the datas before 2018 and one for the datas after; either we will focus our attention on one of the two or we will have to find a way to merge them.
We'll need to define a function in order to quantify healthiness and to add a new column calculating the one of each establishment.

# A list of internal milestones up until project milestone 2
 
- (1st week) Clean the dataset : manage the duplicates, the multiple occurences for an establishment due to multiple inspections, adapt the violations column form to the analysis, find a solution to handle the out of business and not located establishements.

- (2nd week) Take a look at the dataset in order to have an idea of the data's distribution :
    - which are the most represented establishments ? Which ones will we study ?
    - what are the most common violations ?
    - how will we implement the healthiness of an establishment ? Take only the risk factor into account or also the type of violation ? If so, how to classify them ?
    - are the locations well distributed or is a ward-study irrelevant ?
    
- (3rd week) Answer the questions (healthiness of public food establishments according to the type of facility, ward and time ; types of violation depending of the type of facility, ward and time ; where the program could focus to improve the global healthiness). Identify if other questions are interesting to be asked.

- (4th week) Create the interactive map (if it's still meaningfull) and the visualization.

# Prospect

The pinn3r dataset could bring informations based on searches by list of keywords and using tools capable to determine if a sentence is positive, negative or neutral (for example SentiWordNet), which could be relyied on to explain some trends in the results obtained through the healthiness defined during the study.

# Questions for TAa
Does our project seem reasonable and interesting enough for the purpose of the exercise and which questions seem most promising (to know what to focus on first) ?
