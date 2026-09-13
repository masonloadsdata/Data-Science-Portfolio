# Do Dragon-Types Really Win Games?

#1. The Question:
Does having at least one Dragon-type on your VGC team correlate with higher win rates?
Or simply put, do having Dragon-types on your team win games?

This project aims to shed light on an obvious question with a not so obivious answer. Dragon-type pokemon have served an important role in competitive Pokemon VGC. They fill offensive, defensive, and support roles that are crucial in battle. But does simply having one increase your chances of winning?

We are more focused on the general scope of the concept, rather than considering every battle and every move that were or could have been made. This is so that everyone can learn from the results without having to feel overwhelmed by the data. Personally, I find it much easier to just find out a yes or no answer but this just views the outcomes of these teams and not the causes themselves.

#Sources
For this project, I used two APIs. The first is Limitless Tournament Platform API, it provides information from previous competitive VGC Pokemon tournaments. It shows us the players, the teams, the matches, and placements which will be important to us later. The second is PokeAPI, which was used to retrieve pokemon that were classified as Dragon-types. Using PokeAPI like this helped us to avoid any name mismatches and unnecessary errors.

# 2. Units 
Variables: 
has_dragon = 0 no Dragon-types are present; 1 = at least one Dragon-type is present.
dragon_count = int how many Dragon-types are present on the team.
won = int player won the match or lost the match.
winner = playerx who won out of a match.
tournament = name of the tournament in which the match happened.
year = year of the tournament happening.

Note: Only natural Dragon-types are considered. This excludes any Tera transformations or Mega Evolutions(unless they were Dragon-type before). The players do have unique IDs so that their records are recorded. The tournaments also registered at least 16 players with six-Pokemon teams.

# 3. Data Cleaning and Preparation
Cleaning the data was simple, due to the help of AI. While I was creating this project, I was learning the ins and outs of data analysis on Jupyter so AI was very helpful. It showed me steps on how to process data and the concepts that appeared as well.

The first thing I did was remove the players that did not have a public team, as I need the team information to conduct this analysis. Then the pokemon on the teams were converted to lowercase so that each indivdual pokemon can one unique name. Using the PokeAPI, I was able to get a list of all the Dragon-type Pokemon and compare it against the players' teams. This is where I introduced the "has_dragon" and "dragon_count" variables to track the presence of Dragon-types. 
Now I Can start cleaning the match data. Matches that had only one player were dropped, because were are only focused on wins that were battled (has two people). I also removed ties and double losses because that were are only focused on wins and losses. Lastly, matches that had both teams containing Dragon-types and matches that contained no Dragon-types were removed from consideration; as they do not compare well in the comparison.

# 4. Visualizations
Data Visual 1: [Dragon Win Rates](https://github.com/masonloadsdata/Data-Science-Portfolio/blob/7d8173a0d409a3ca3a5cf2b378eb9ab45bdb7622/Projects/VGC%20Dragon%20Analysis/output0.png)

Data Visual 2: [Dragon Type Win Rates in Tournaments](https://github.com/masonloadsdata/Data-Science-Portfolio/blob/f6a89751f4012e6ec07f9f67b451f57313179d9f/Projects/VGC%20Dragon%20Analysis/output1.png)

# 5. Findings
Our central question is based on if Dragon-type Pokémon and winning are associated. Data Visual 1 tells us that it wins 43.75% of the time compared to a 50.0% baseline. Ideally to win tournaments and championships, you want to win more than 50% of the time, because you can't place first if you don't win more than you lose. However the p-value obtained from the statistical test presents a .8036, which means that about 80% of the data could be random chance or extreme. This is important to note because the chart shows that Dragons-types win at a 43.75% rate but the a large chunk of the data could be just random chance. With these findings, there is no proof that Dragon-types are the ultimate key to winning. 

# 6. Limits, Ethics, Reflect
One of the major things about this whole concept is that players register a six-Pokémon team, but only four are fielded per battle. This means that even though our data is based on the six-Pokémon teams, we cannot see which were used in battle. 

Another thing about competitive esports is that the META changes. META is an acronym for "Most Efficient Tactic Available", which as it says it is the best method of winning. The developers at Nintendo and many other games studios design their games so that as they push out updates, the competitive environment changes. Think of this like a game of basketball but as a few months or a year go by the game changes, like the basket moves to the corner instead of the middle and the ball gets twice as big. Changes like these happen all across competitive esports scenes. In the context of Pokémon, the regulations change as new games, abilities, items, and Pokémon are released.

With more time and data, I would expand my project in one general direction. 
I'd examine each individual Dragon-type, investigate which specific Dragon-type Pokémon is the most impactful across many games. I would also look at what moves the Pokémon know and how often they are used.

# 7. Code and Transparency

Jupyter Notebook: [Code](https://github.com/masonloadsdata/Data-Science-Portfolio/blob/7be3ca2c14acea4dcf021ae0003e9f0a6629605f/Projects/VGC%20Dragon%20Analysis/Project%201%20Pokemon.ipynb)


