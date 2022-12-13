# LoL_Data_Analysis

**About the project**

This project started from my interest in games, especially a game named League of Legends. Since I was both interested in the field of data analysis as well as League of Legends, doing a project that relates the two fields would be interesting. Through this data analysis, I aimed to come up with new information. I would also like to create some analysis and compute the conditional probability showing one condition’s likelihood of happening given the other condition. 

From Kaggle, I obtained the data about three main areas: champion, spells, and game. I included different information from each data. The champion data contains champion id, the name/title of the champion, and their tags (ex. fighter, tank., support, marksman). These tags refer to the actual tag within the game. Spell data contains the information about spells: it contains the name, key, and the description of each spell. games.csv includes information about individual games: they contain information about individual games, such as “champions that are used,” “which team took the first Dragon”, “first Tower”, “first Baron”, “first Rift Herald”, “first Tower”, “firstBlood”, and “which team won”. 

**Data Background**

I chose this data because I had a deep interest in the game League of Legends. In this game, objects take huge importance. Each object is defined, and they are Rift Herald, Dragon, Baron, and Tower. Each of the four objects help the team to win, with the Rift Herald being important in the early stages of the game, and Dragon, Tower, and Baron becoming important in the later stages of the game. Each of the four objects are worthy of investigation in terms of data analysis. 

**Initial Data Exploration/ Visualization **

First, as all data analysis does, I started with data exploration, exploring the given data about games, champions, and spells. With the imported data, I converted each json and csv file into a form of dataframe, which is easier to implement pandas and thus allowing for more in depth analysis.

In Data_Exploration_Final.ipynb, I imported all the data needed for my data analysis and conducted sanity checks to confirm that all of our data sets contain valid values. After the sanity check, I went into visualization and in depth analysis. 

In Visualization_Final.ipynb, I used a different pandas function to filter out only the relevant columns, which were the information about Baron, Dragon, Rift Herald, and Tower. Using this data, I visualized the new dataframe into bar graphs and pie charts to compare the number of games in which the teams were involved in taking the objects. 

**Conditional probability/analysis**

In the Conditional_Probability_Final.ipynb, I used the pandas functions to count joint events. After counting the number of games for each condition, I created a probability table that allowed me to give insights about how taking a certain object influences other key events. Most of the objects listed above (Baron, Dragon, and Rift Herald) contributed significantly to the team’s victory, while first Blood and first Tower contributed less. From looking through my analysis and calculations, I came up with the following conclusion: Rift Herald, Dragon, and Baron boosted the win rate more than first Blood and first Tower. Out of the three most important factors for a team winning, Baron was the most important, giving a team more than 80% chance of winning when taken. 

In Analysis_Final.ipynb, I used pandas functions to calculate all the win rates for individual champions, and placed them in a list for better visualization. Then, using the data from the binomial test, I divided the champions into two cases of win rates: over 0.5 (50%) or under. For champions that have a win rate over 53%, I organized them into another list to indicate they are good champions to use. Because there were some champions that did not use a list of win rate < 0.5, I also compiled all of those champions into one list. From the champions, only 17 champions were not used, and only 10 champions had good winning rates. 

**Conclusion/ overall insight**

The overall conclusion is that for a team to win a game, a team should focus on first Rift Herald, Dragon, and Baron. From my prior knowledge of the game, this is because first Tower and first Blood could always be overcome in the middle stages of the game. Even if a team takes first Blood, winning a certain lane, the opponent team always has a chance to win the other lanes and flip the tides of the game. This also applies to the first Tower. However, Rift Herald or Dragon is an object that could be used to lead the team into victory. This makes them more dominant in strategizing the team's victory. In the case of Baron, this object boosts the ability of the minion and plays a critical role within later stages of the game. This is the reason why Baron takes a significant portion in a team winning. 

From Analysis_Final.ipynb, I was able to figure out what champions are good to use based on the winning rate. These champions were: Anivia, Garen, Janna, Rammus, Sejuani, Shyvana, Singed, Sona, Swain, and Yorick. There were also champions that were not used at all: Aurelion Sol, Cho'gath, Dr Mundo, Jarvan IV, Kha'zix, Kog'maw, Leblanc, Lee Sin, Master Yi, Miss Fortune, Monkey King, None, Rek'Sai, Tahm Kench, Twisted Fate, Vel'koz, and XinZhao turned out to be the unpopular champions. This is most likely because of the meta of the game, where certain champions become good and other champions become useless based on the change in game meta. However, based on my background knowledge of the champions, another potential  reason for certain champions’ high win rate is based on the users of that champion. Since most of the champions listed with a win rate above 53% are champions that are only used by masters, they consequently have a higher chance of winning. 

**Evaluation**

While I did this project, I met some limitations due to the time constraint. Even though I had data about spells,  I was not able to connect this data to my analysis and talk about it. Given more time, I also would have explored spell data more. Given more time, I also would have explored spell data more. This would diversify my conclusion, and add more information.  


