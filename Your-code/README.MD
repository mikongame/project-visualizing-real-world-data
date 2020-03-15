<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100" align="right"/>


#   Project Ironhack Data Bootcamp: Visualizing Real World Data

MIGUEL GARCÍA MELGAR

*Data Part Time Barcelona Dic 2019*


## Content
- [Project Description](#project)
- [API](#API)
- [Web](#web)
- [Workflow](#workflow)
- [Results](#results)

<a name="project"></a>

## Project Description

### Overview

The goal of this project was to practice creating and interpreting different types of visualizations using real world data, yet I decided to use the data I cleaned and transformed for the previous project.


### Technical Requirements

The technical requirements for this project are as follows:

* We had to select a dataset from a public source but, despite being in a public github repo, we used the datasets resulting from the previous project.
* We created a Jupyter noteboosk to analyze the data.
* Using our data, we tried to create a at least of one scatter plot, one histogram, one box plot and one bar graph. Graphs should contain the proper labeling of the x and y axis when appropriate as well as a title for the graph.
* Explain what insights can be inferred from these visualizations. The explanation should be in the notebook in markdown cells.

### Necessary Deliverables

The following deliverables were pushed to our Github repo for this chapter.

* **A Jupyter Notebook** containing the analysis and the code used to obtain this analysis.
* **An data folder** containing the datasets
* **A README.md** containing a detailed explanation of the followed approach visializing and analysing the information.

<a name="Datasets"></a>

## Datasets
 
* The datasets we'll use are 4 csv files: pikalyticsDF_clean, cointaining the cleaned information resulting from using pikalytics API; wikidexDF_clean, that includes cleaned information obtained from wikidex web page; Combined_DF_clean, that combines the previous datasets; and outliers_clean, which states those pokemon that are very rarely used in VGC 2020. It is to be noted that we we'll focuse on the 2 latest.
* If we have time enough we will use Parsehub to scrape information from Pokémon World Championships official results on pokemon.com from 2014 to 2019 so as to create a new dataset joining and listing the top 8 contestants' teams of masters, senior and junior categories.
  
<a name="workflow"></a>

## Workflow

### Import Useful Libraries

### Pikalytics dataset
#### Pikalytics dataset EDA and cleaning
#### Pikalytics dataset visualization
#### Pikalytics dataset insights

### Wikidex dataset
#### Wikidex dataset EDA and cleaning
#### Wikidex dataset visualization
#### Wikidex dataset insights

### Combined dataset
#### Combined dataset EDA and cleaning
#### Combined dataset visualization
#### Combined dataset insights

### Outliers dataset
#### Outliers dataset EDA and cleaning
#### Outliers dataset visualization
#### Outliers dataset insights

## Conclusions

##### ¿Does viability predict usage?

We don't really know if *viability* predicts *usage*, or if it is the latest that defines which Pokémon deserves to be in which *viability* cluster. However we can see that the 3 most used Pokémon are in cluster B, cluster B- Pokémon are used almost as much frequently, and very few Pokemon within-cluster C+ are used, being 0 Pokémon from lower strata. 

Still, we don't know what are the rules deciding in which stratum Pokémon are classified and... ¿What about A, A-, and B+ clusters? ¿Are they *Uber* (banned)?

##### Comment about Base Stats distribution through the whole list of Pokémon.

`Shape:`
All the distributions are right-skewed, slightly in *Attack* and *Speed* instances, which are closer to a normal distribution; but none is Wald distributed as they had no support on (0,∞). 

`Centre:`
The stat with the highest mean is *Attack* (80.11) whilst the lowest is *Speed* (67.96) being all-together with *HP* (69.53) the only stats with below overall stats mean (72.78) means.

`Spread:`
The stat that holds the biggest spread is *HP* (1-255) whereas *Speed* (5-180) has the lowest range of values.

`Kurtosis:`
Defensive stats (*HP, Defense and Special Defense*) seem to be more Leptokurtic, especially *HP*. On the other hand, offensive-related base stats are more Mesokurtic, being *Speed* the best example.

##### Comments about VGC 2020 Usage % and Base Stats Mean relationship

Pokémon's usage in VGC 2020 online competitions seems to be ***positively correlated*** with each Pokémon's Base Stats Mean forming a ***logarithmic growth*** so that Stats Means grow a lot without affecting much to VGC Usage %, and from 70 base stats means, usage starts increasing really fast, and it almost stops growing from 85-90 mean values.

##### Comment about Base Stats distribution of Pokémon very rarely used in VGC 2020
`Centre:`
The stat with the highest mean is *Defense* (62.13) whilst the lowest is *HP* (46.94) being all-together with *Speed* (48) being below average (54.67) as *Special Attack* (52.94).

`Spread:`
The stat that holds the biggest spread is *Defense* (24-135) whereas *Speed* (16-75) has again the lowest range of values.

`Outliers:`
Among all outliers, there's just 2 that are not in this dataset because of having much lower Base Stats Mean that the other competitive Pokémon: Shedinja and Stonjourner. The first one is here because of its negligible HP (1), the latest because of holding the lowest Base Special Defense among Pokémon frequently used in VGC.

Actually, all those data come from those Pokémon that are outliers among VGC 2020 used Pokémon, still there 2 outliers among them. 

One of them is Shedinja which can be considered an outlier among outliers because of its HP (being 1). The other one is Stonjourner, outlying because of both its high HP (100) and its high defence (135).
