#Analysis Breakdown: Predicting Destiny 2 Steam Player Engagement

##1. Problem Definition

Recently, Bungie and Sony have been having a very big problem involving the Destiny 2 IP, their newly laid off employees, and outraged fans. What I want to address is what factors contribute mostly to Destiny 2's seasonal success, this means that our target variable will be "next_month_avg_players" and that our problem will include a regression model. The people benefiting from this study range from the people that develop the game and push out updates to the fans enjoying the game. Really it is a cycle because the better the studio the more the fans will pay for the game. Bungie is one of the many studios that updates their games to the fans' reviews, and if other studios can implement this data to their games then perhaps more games will be more enjoyable. 

##2. Background and Context

Destiny 2 is an MMORPG(Massively Multiplayer Online Role Playing Game) that progressively gets updates every month and major updates every year. Sony is the entertainment company that owns Bungie, and Bungie is the studio that created and maintains Destiny 2.

AI Provided Context:

Prior research supports treating game engagement and community response as measurable phenomena. Hamari and Keronen (2017) synthesize research on motivations for game use. Zhu and Zhang (2010) find that online consumer reviews can influence video-game sales, while Kraemer, Weiger, and Heidenreich (2025) report nonlinear relationships between review valence and video-game sales. These studies do not establish that Steam review sentiment causes Destiny 2 player activity, but they support examining reviews and engagement-related indicators as predictive features.

##3. Data Description
The data used for the model comes straight from Steam and Bungie. 



Hamari, J., & Keronen, L. (2017). Why do people play games? A meta-analysis. International Journal of Information Management, 37(3), 125–141. https://doi.org/10.1016/j.ijinfomgt.2017.01.006
Kraemer, T., Weiger, W. H., & Heidenreich, S. (2025). Do all stars shine the same? Investigating the nonlinear effects of user and critic reviews on video game sales. Journal of Business Research, 188, 115034. https://doi.org/10.1016/j.jbusres.2024.115034
Zhu, F., & Zhang, X. (2010). Impact of online consumer reviews on sales: The moderating role of product and consumer characteristics. Journal of Marketing, 74(2), 133–148. https://doi.org/10.1509/jm.74.2.133
Valve Corporation. (n.d.). IUserReviewsService. Steamworks Documentation. https://partner.steamgames.com/doc/webapi/IUserReviewsService
Valve Corporation. (n.d.). ISteamNews interface. Steamworks Documentation. https://partner.steamgames.com/doc/webapi/ISteamNews
Steam Charts. (n.d.). Destiny 2. https://steamcharts.com/app/1085660

