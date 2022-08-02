# All-time NBA and MLB Players by Birth State

**OBJECTIVE**: Analyze the number of all-time players for both NBA and MLB by the State where they were born. Which State delivers the most basketball and baseball players? From which region do most professional players come? (Considering only the United States)

## Table of Contents

- [Data Description](#datadescription)
- [Data Preparation](#datapreparation)
- [Visualizations](#visualizations)
- [Comments](#comment)


<a id='datadescription'></a>
## Data Description

##### NBA
Kaggle dataset: https://www.kaggle.com/datasets/drgilermo/nba-players-stats?datasetId=1358&select=Players.csv (Players.csv)

**Number of Instances**: 3922

**Number of Attributes**: 7 features, 4 text columns and 3 numerical attributes

**Attribute Information**: Player: player's full name (first and last); height: height in cm; weight: weight in Kg; collage: college attended by the player; born: birthdate of the player; birth_city: city where the player was born; birth_state: state where the player was born 

##### MLB
Kaggle dataset: https://www.kaggle.com/datasets/seanlahman/the-history-of-baseball (players.csv)

**Number of Instances**: 20358

**Number of Attributes**: 24 features

**Main Attributes Information**: birth_year: birth year of the player; birth_country: country where the player was born; birth_state: state where the player was born; birth_city: city where the player was born; death_year: death year of the player; death_country: country where the player died; death_state: state where the player died; death_city: city where the player died; ...

##### Population
Wikipedia table: https://en.wikipedia.org/wiki/List_of_U.S._states_and_territories_by_population (table-1)

**Number of Instances**: 61

**Number of Attributes**: 16 columns

**Main Attributes Information**: State or territory: State name; Census population: census population by State (different columns for different census years)


<a id='datapreparation'></a>
## Data Preparation
We consider only players born in the US for the NBA and MLB data. Missing values in the birth state columns are dropped. For the population data, we consider each State's census conducted on April 1, 2020. After merging all three resulting datasets by State, compute the number of players in a million people for each State. The choice for such transformation is linked to a much easier comparison and interpretation and less sparse visualizations. Add also a 'Region' column, which for each State contains the corresponding region.


<a id='visualizations'></a>
## Visualizations
* Scatterplot with values by State

![newplot](https://user-images.githubusercontent.com/80990030/182402966-0fe8e3bc-a724-40d4-9108-77a6eb83f95a.png)


* Barplot with values by Region

![newplot1](https://user-images.githubusercontent.com/80990030/182403010-5d02b17f-087f-41b8-815d-11e026cef0d5.png)


<a id='comment'></a>
## Comments
The two main visualizations allow us to compare different States and Regions.
The similarities and differences between States and Regions could be due to: 
* Cultural aspects: like the appeal of a particular sport
* Climatic aspects: weather conditions may influence the preponderance for indoor/outdoor sports
* Institutional: like better sports programs and schools
* Demographic: population's age distribution, etc. 
* Many other possible causes and explanations
