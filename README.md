# WC22_Pred: Qatar 2022 Prediction
Predicting the Qatar 2022 World Cup winner from the Round of 16 games.

## Methods used
Normalized 50% FIFA ELO + Normalized 50% "Power Rank" (form rank in Qatar 2022), then used to find the [cumulative distribution function](https://en.wikipedia.org/wiki/Cumulative_distribution_function) coefficient. cdf of each team is used as weights in predicting the winner of a match.

## Calculating the Power Rank
For every match where it's deemed important, Power Rank is calculated from subtracting the square root of the expected goal of the team (xG) from the square root of the actual goal (score).

### Credits
Scraped match data is from https://fbref.com.
FIFA ELO is from https://eloratings.net.