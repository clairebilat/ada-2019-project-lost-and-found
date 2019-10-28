# Where to eat in Chigago : an analysis of the inspections from Chicago department of Public Health's Food Protection Programm

# Abstract
The Chicago department of Public Health’s Food Protection Program provides a database derived from inspections of restaurants and other food establishments in Chicago from 20120 to the present. It contains many information about the establishments, like the type of facility (groceries’ stores, restaurants, coffee shop, …), and its location. Many information about the violations detected there are also provided there, like the reason that led to the inspection.
In our project we endeavor to visualize the healthiness of public food establishments according to the type of facility or its ward. An analysis of the violation’s type according to the facility’s type and the facility’s ward will also be conducted. 
The purpose of the project is to help the consumer to easily choose where to eat in Chicago, but also help the Chicago department of Public Health’s Food Protection Program to adapt their response and work (for example, where should a prevention program be proposed).



# Research questions
How to exercise the appropriate precautions when viewing or analyzing these data in order to manage the duplicatas ?
How to implement a good vizualisation tool (with an interactive map for example) ?
How to take into account that an esthablishment has multiple violations ?


# Dataset
List the dataset(s) you want to use, and some ideas on how do you expect to get, manage, process and enrich it/them. Show us you've read the docs and some examples, and you've a clear idea on what to expect. Discuss data size and format if relevant.

# A list of internal milestones up until project milestone 2
Add here a sketch of your planning for the next project milestone.

# Questions for TAa
Add here some questions you have for us, in general or project-specific.



Example 1 : 

Social topics throughout music: sentiment analysis
Abstract
In this project, our goal is to find out about the social topics evolution in culture. We will use music lyrics from the “Million song dataset” to analyse sentiment in tracks from artist, genres and time. What can the sentiment towards different topics in songs tell us about people and the time they live in? Our goal is to provide a visualization of semantic trends in music, that hopefully will give people more insight into everyday social topics and how they evolve as a part of our culture. To visualize our data, we want high interactivity so one can have filter by one’s own interest in this high dimensional space. Therefore, our work will be presented in the form of an interactive blog.

Research questions
We will guide our work with the following questions:

How is the perception of certain topics evolving throughout time and within genres?
How is the relationship between topics and locations characterized in different music genres?
Is there a correlation between the complexity of lyrics and specific topics?
Dataset
Our main dataset is coming from the one called “Million song” that was provided with the project list. As specified in the abstract we will be working on the lyrics with the “musiXmatch” dataset and the “tagtraum” dataset for genres. We might use the “Top MAGD” dataset that gives more music genres, it depends on how performant we manage to be with the first genre dataset. We will also use NLTK to analyse whether the words/sentences that are used are of a positive or negative nature. To get additional specific information from artists, like pictures and origin, we will use Wikidata

A list of internal milestones up until project milestone 2
04.11

Download the required data
Set up the Git and project skeleton
11.11

Establish the sentiment analysis on all the song of our dataset and create a new table
Append an additional rating to the positive/negative one that is provided by NLTK
Find the most powerful way to store and look up all our data
Find how we can clean our dataset
19.11

Explore possibilities for the data visualization
Decide which visualization format is the best.
Characterization of the artists and lyrics in genres and grouping
Use the data from WikiData to get extra information such as pictures or precise artists’ origins
26.11

Comment and debug our code
Set up our goals and plans for the next milestone.
Options to consider:
Extend our work to others languages than English
Questions for TAa
Are we allowed to use pictures for representation of artists if our work is not publicly published? Copyright-wise, how does this work?
Is the content we have enough to make a project?
Is the idea fitting to the “social good” topic?
In terms of visualization and analysis, which aspect is the most important one?



Example 2 :

Title
Evolution in music through the years.

Abstract
The music world is constantly increasing with lot of songs published everyday from all over the world. Moreover, the world is becoming more connected and this helps to spread music popularity. We want to understand how music popularity evolved in the last roughly 60 years, as music is a really important social factor. People express themselves, and lot of cultural events and customs are derived from it. This popularity could help explain some movements influence, the creation of some music styles and what makes a song popular. If there was a "perfect" composition it would be interesting as it has also become a money-making industry. We will use the dataset from MillionSongDB, coupled with some website such as The Echo Nest API (now Spotify) and musicbrainz.

Research questions
Which features did change (e.g. bpm, beats)?
How did genres change (e.g. popularity, features of specific genres, higher variance)?
How did the distribution of music change (e.g. change of number of genres, variance of features)?
Which songs from the past are still trending (why)?
How did song titles (artist names) change over time?
Where did (which) songs get released at which time (do dependencies exist between similar Songs)?
Dataset
We want to use the dataset from MillionSong DB.
It consist of .h5 files containing song, classified in different subfolders. For each .h5 files, we can use the method given in the hdf5_getters provided by the website to extract useful information. The most important one is the .get_num_song(file) that return the number of rows in the actual files, then you can get lot of information on the artists, songs, etc. The fields that could be exploited are mentioned on the following wepage in the field list paragraph: https://labrosa.ee.columbia.edu/millionsong/faq .
Furthermore a few additional files with aggregated data (e.g. longitude, similarities, year) can be bundled via offered scripts: https://labrosa.ee.columbia.edu/millionsong/pages/getting-dataset.
Genres are called "terms" in the dataset. The genres of an artist can be fetched from the field "artist terms". Or from one of the additional files. There are several features which have been calculated with algorithms: BPM ("tempo"), dancabilty, duration, etc. Possibly further facts can be retrieved from the Spotify API since the Echo Nest API is shut down.
Since the dataset is quite large and we will start to look in the additional files to get as much simple information as we can. Furthermore, a subset exits, which we can use for first tests. Later on, we can fetch additional information from the whole data set.

A list of internal milestones up until project milestone 2
03.11.2017: Prepare subdataset locally

05.11.2017: Analysed additional files

10.11.2017: Fetched data from subdataset and APIs, create functions for additional data collection

17.11.2017: Functions created for explanatory data analysis on subdataset

19.11.2017: Prepared complete dataset on cluster

24.11.2017: Applyed created functions on whole dataset, do needed modifications

26.11.2017: Extended functions and analysis for whole dataset, prelimiary result

28.11.2017: Rechecked prelimiary result, updated plan

03.12.2017: Relevant conclusions drawn

08.12.2017: First blog design

15.12.2017: Data visualisation

19.12.2017: Finalized Data Story and notebook

29.01.2018: Create poster, demo of visualisation

Questions for TAa
Is there a possibility to convert IDs from the dataset to Spotify URNs?



Example 3 :

Mental Health in Switzerland
Abstract
Social media, such as Twitter, provide a unique look into people’s feelings and thoughts. As such, aggregated data from social media has previously been successfully used to identify depression and other mental illnesses in users. However, most studies on this subject tend to focus only on clinical depression, which is a very specific condition that is not indicative of the general mental health of the population.

Switzerland has one of the best mental health infrastructures, indicating that mental health probably is a problem within the population. Nevertheless, society still stigmatizes these issues, which is why we turn to social media to get a better picture of mental health in the country by focusing on more general indicators of mental health disorders. We use simple natural language processing methods to get more insights into the affected population and how they are perceived by Swiss society.

Research questions
Mental Health : where we stand
What indicators of mental health issues can we find in tweets?
What percentage of tweets / how many accounts show such indicators?
Can we find seasonal patterns? Winter VS Summer? (Seasonal Affective Disorder)
Can we see regional patterns? Countryside VS city? Can we find increased levels of mental illness indicators around high stress areas such as EPFL?
To what extent is Twitter representative of the country’s health census?
Mental Health: what we think about it
Can we identify stigmatization of mental health based on tweets and the news?
If so, to what extent is it present?
How has this image changed over time?
Dataset
Datasets we want to use
Swiss tweets dataset (to get the tweets from the general population).
200 years news (however, ends in 1998) (to get the sentiments from media, use the SPARQL Endpoint).
Methology
Data exploration, check if we can actualy find any issues with twitter data and make sure to handle them. (For example depression can be used in an economic way).
Use simple natural language processing methods (LSI, pLSI, LDA and VSM using lemmatization, stemming and n-grams) to preform analysis on data set.
Determine a dictionary of keywords linked to mental health and emotion identifiers (and possibly (if time allows) use Machine Learning algorithms to broaden it along our work).
Filter tweets by the dictionary and construct a dataset we can work with on. Such as, number of tweets containing dictonary entry by region, season, language.
Find trends allowing us to broaden our research or tweak our model to iterate on those steps.
Use the news data set by using keywords from the dictionary (previously built).
A list of internal milestones up until project milestone 2
1. Handle the raw data & general data analysis (to be done before nov. 12th)
Check how we get data on our computer and how we can handle the large volume of data.
Learn how the dataset is encoded, how specific the geomarkers are, and if sentiment stamps are useful to our question.
Look at the overall distribution of the tweets' languages, and check for issues with non-standardization of Swiss German. -> also look at regional distribution.
Look at how frequent the use of emojis is, what methods to use to handle them.
Look into handling time dimension of data, look at distribution of tweets over time.
See to what extent Swiss News outlets talk about mental health.
Find potential issues with data, are there any NaN values, how can we deal with bots and spam etc. (*Read papers that might give us interesting insights)
2. See how we can transform the data (to be done before nov. 18th)
Look more closely into what NLP techniques work best on our data and begin to form our dictionary.
Filter the tweets down to a dataset that interests us, check if size of dataset is reasonable.
Check how we can look at the tweets in a temporal manner, what statistical tools we should use to be able to draw conclusions.
Look into ways we can visualize our data.
3. Work on notebook and future plans (until deadline nov. 28th)
Work on properly commented notebook that can be read by people outside the team.
Have a nice visualisations and first results in notebook.
Questions for TAs
What is a good scope of the projet, e.g. is our project too ambitious or not ambitious enough? -> The mental health stigma part might be too much and we weren't sure if we should include it or not/or instead center our project around it. -> What are the 'expecations'?
Regarding the second step of our methodology, can we use external libraries or help to define the dictionary?
How should we best get data from the 200 years news source, how can we deal with the issue that it only covers francophone media? Can we use other new sources to have more recent data (same time as tweets)?



Example 4 :

Backtracing Innovation
From Snapchat's Facial Recognition to the Inception of Semiconductors

Abstract
The US Patent & Trademark Office, short USPTO, offers a full-fledged directed graph of US patent citations since 1975. Many at the time obscure patents paved the way for groundbreaking new technologies in the future, as for example Google's Page Rank (#6285999) or Apple's touch screen devices (#7479949). In our project we endeavor to visualize this massive graph with more than 89 Million edges in an appealing and concise way in order to render the narration of more intricate stories possible and offer potential users a slick and interactive interface for navigating the patents graph. Inspirations on how to beautifully draw a graph network are taken from Kirell Benzi. Those stories may range from analysing node connectivities to extract influences of particular inventors to finding the shortest walks between patents. Through this we hope to gain deeper insight into the metastructure of inventions throughout the digital revolution and how they shape the future as we know it today.

Research questions
How to apply common graph algorithms to a massive data set?
How to efficiently travers and query a graph of that scale?
How to visualize a large and complicated graph?
How to handle missing edges in the patent graph?
How to eliminate equal patents that were filed under several identifiers?
How to draw conclusions about technology soley given patents and their citations?
Datasets
USPTO patents database
Google patents
Internal milestones up until milestone 2
Refresh on graph algorithms.
Look for efficient graph processing libraries. Preferably with GPU integration.
Sight data and perform preliminary analysis.
Find blog skeleton.
Discuss narrative of the data story.
TA Questions
What technologies do professional data blogs like FiveThirtyEight use for visualisation?
What is Kirell Benzi's magic library?
