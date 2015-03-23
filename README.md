# cricket-wc2015
=======
Ball-by-ball data for all matches of the 2015 cricket world cup (till the quarterfinals). The scripts used to scrape and clean this data have been kept private to ensure that they are not abused.

The files that you can use for analysis are in the wc_cleaned_data folder. These files create ball-by-ball details for individual games. The data for a game with the game id <x> is stored in <x>_summary.csv

Below is a summary of what some of the headers in the summary file entail:
- 'batsman' refers to the player id of the batsman
- 'bowler' refers to the player id of the bowler
- 'bat_right_handed' indicates whether the player is left or right handed
- 'x' and 'y' refer to the coordinates of where the ball ended up after it was hit.
-   'x' is 0 when it reaches the left-most region of the ground (the point boundary for a right hander) and is 360 when it reaches the right-most region of the ground (the point boundary for a right hander).
-   'y' is 0 when the ball reaches the boundary straight down the ground (i.e., after a perfect straight drive), and is 360 when it reaches the boundary after going over the keeper's head
- 'z' refers to the zone in which a ball was hit. z=1 is the fine-leg zone, z=2 is the zone behind square leg, z=3 is the zone in front of square leg etc. This progress all the way until z=8, which is the third-man area.
- landing_x refers to the distance (in meters) away from the centre of the pitch that the ball lands. A negative value indicates the ball landed outside off-stump for a right-hander and outside leg-stump for a left-hander.
- landing_y refers to the distance (in meters) away from the batsman stumps that a ball lands. A negative value indicates a full toss.
- ended_x refers to the distance (in meters) away from the centre of the pitch that the ball ends up when it reaches the batsman. A negative value indicates the ball landed outside off-stump for a right-hander and outside leg-stump for a left-hander.
- ended_y refers to the height (in meters) above the pitch by the time it reaches the batsman.
- ball_speed refers to the speed of the ball in miles per hour
- control refers to whether or not the batsman middled the ball (1=middled, 0=not middled)
