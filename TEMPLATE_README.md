# Movie Analysis for Microsoft

**Authors**: Hyunwook Paul Shin, Derek Supino and Stephen William

https://images.squarespace-cdn.com/content/v1/5817f843579fb366cecb8e9a/1610030522633-QNYMAAV89SWZ97BJW46C/theater.jpg?format=1000w


## Overview

This is a project to provide Microsoft with a guide on what goes into creating and releasing a sucessfull movie based on data pulled from several reputable sources. Microsoft has launched its own movie studio but they don't know what tpye of film to release or even who to hire to help create a profitable film. The data was cleaned, organized and analysised to find out what the most sucessfull films of all time had in common with each other. With this information we can present the head of Microsoft's new movie studio what they can do to guarentee a sucessfull movie release.


-----A one-paragraph overview of the project, including the business problem, data, methods, results and recommendations.

## Business Problem

Micosoft's new film studio has just launched and they are trying to release a sucessfull movie but don't know where to start. With the data we collected and analysed we where able to come up with some questions that we thought where important to a sucessfull movie like "What months generate the most worldwide gross?", "What genres brings in the most profit?", and "What directors have brought in the biggest profits?". We believe these are the most important questions for a new film studio to ask because overall these are variables that can be closely connected to generating a profit.

We have 3 deliverables for the directors of the Microsoft Studio:
* Suggest which types of films are worth focusing on by establishing which genre makes the most profit.
* Analyze the monthly average return on investment rate for the suggested genre to determine which month has the best chance of earning profit.
* Evaluate how much do the top 50 directors contribute to the total profit to study the impact of the director on the movie production. 


-----Summary of the business problem you are trying to solve, and the data questions that you plan to answer in order to solve them.

***
Questions to consider:
* What are the business's pain points related to this project?
* How did you pick the data analysis question(s) that you did?
* Why are these questions important from a business perspective?
***

## Data
We will use the data from the following sources:
* __[IMDB](https://www.imdb.com/)__
* __[The Numbers](https://www.the-numbers.com)__

IMDB: There are multiple dataset only including partial informations. The information we will need for the most is the genres and the staffs (directors, writers, actors, production) involved in movie production. 

The relevant dataset we will be using are the followings: 

* `imdb.name.basics.csv.gz`
* `imdb.title.akas.csv.gz
* `imdb.title.basics.csv.gz`
* `imdb.title.principals.csv.gz`

The Number : This dataset includes the production budget and gross profit (both domestic and worldwide). The release date of the film is also included. The economic metrics will be used further to calculate the net profit and return on investment ratio (ROI).

The relevant dataset we will be using are the followings: 
* `tn.movie_budgets.csv.gz`

----Describe the data being used for this project.
Data was collected from the following websites:
    -https://datasets.imdbws.com/
    -https://www.kaggle.com/stefanoleone992/rotten-tomatoes-movies-and-critic-reviews-dataset?select=rotten_tomatoes_movies.csv
    


https://www.kaggle.com/stefanoleone992/imdb-extensive-dataset
https://www.imdb.com/interfaces/





***
Questions to consider:
* Where did the data come from, and how do they relate to the data analysis questions?
* What do the data represent? Who is in the sample and what variables are included?
* What is the target variable?
* What are the properties of the variables you intend to use?
***

## Methods

-----Describe the process for analyzing or modeling the data. For Phase 1, this will be descriptive analysis.

The several Imdb data sets where connected using movie and crew ID's to connect movie titles with their correct release date, budget, gross, crew members and genre's. Some data was missing so we further connected the movie titles and crew names with other data sets from Rotten Tomatoes and Numbers.com. With this method we can consolidate the data into just a few usefull tables that make it easier to analyse and cut out data that we don't find usefull. 



***
Questions to consider:
* How did you prepare, analyze or model the data?
* Why is this approach appropriate given the data and the business problem?
***

## Results
### Genres with Top Average Net Profit
![graph1](./Visuals/Top_Genre_Profit.png)

### Monthly Average ROI over the year
![graph2](./Visuals/Monthly_ROI.png)

### Impact of Top 50 Driector
![graph3](./Visuals/Total_Profit.png)
--------Present your key results. For Phase 1, this will be findings from your descriptive analysis.

The results that we came up with based on our analytics is when is the best month to release a movie of a certain genre that typically brings in a large worldwide gross. We came to these rusults by finding the genres that produce the most profit and find the best performing months for those genres. So we can recomend to Microsoft that making an Animation movie will most likely generate a profit and to ensure that the movie will perform as best as it can we can also recomend that Microsoft release an Animated film in the month of June because based on historic data, Animated movies bring in the most Box Office Gross in the month of June. 

Another result that we came up with is what directors are associated with generating the most profits. Through our analysis we discovered that the top 50 directors based on movie profits is responsible for 46% of total box office profits across all movies in our datasets released since 2010. 





***
Questions to consider:
* How do you interpret the results?
* How confident are you that your results would generalize beyond the data you have?
***

Here is an example of how to embed images from your sub-folder:

### Visual 1
![graph1](./images/viz1.png)

## Conclusions

Provide your conclusions about the work you've done, including any limitations or next steps.

***
Questions to consider:
* What would you recommend the business do as a result of this work?
* What are some reasons why your analysis might not fully solve the business problem?
* What else could you do in the future to improve this project?
***

## For More Information

Please review our full analysis in [our Jupyter Notebook](./dsc-phase1-project-template.ipynb) or our [presentation](./DS_Project_Presentation.pdf).

For any additional questions, please contact **name & email, name & email**

## Repository Structure

Describe the structure of your repository and its contents, for example:

```
├── README.md                           <- The top-level README for reviewers of this project
├── dsc-phase1-project-template.ipynb   <- Narrative documentation of analysis in Jupyter notebook
├── DS_Project_Presentation.pdf         <- PDF version of project presentation
├── data                                <- Both sourced externally and generated from code
└── images                              <- Both sourced externally and generated from code
```



Commit History:

First 45 commits consisted of setting up the main repo, all group members branches and organizing of files and folders. 
set up Main jupyter notebook and one for each team member. 
unzipped data files and deleted old unused files. 
changed "zippedData" folder to "Data"
README.md updated with info on source of data 
Branch Stephen added Jupyter Notebook containing cleaned TMDB movie data containing release dates
Branch Stephen organized files into seprate folders.
Branch Stephen push to main
On Main Branch git commit -m "added .ipynb_checkpoints and DS_Store to .gitignore"
On main branch git commit -m "moving .ipynb_checkpoints to .gitignore"
From Branch Derek push Movie_Project_Draft.ipynb to main
Main branch merged with branch Stephen
git commit -m "adding 3in1 bar chart"
git commit -m "graphs and charts saved in visuals"
Paul Branch Push Movie_Project_Draft updated with 3 in 1 bar chart


