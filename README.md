## Introduction

College football is a game enjoyed by millions of fans across the country in the fall.  Part of the uniqueness of college football, unlike the pros, is that each player
decides where they want to go to school, so the recruiting process plays a big part in how the teams perform on the field each week.  The better players you can recruit
to your school, the more likely you are to have a winning team during the season.  Players can redshirt in college, so they have a chance to develop over five years, so
you have to look at the recruiting across that time period to see if the players you brought in over that time worked together on the field to acheive success.

## Problem Statement

I want to understand how much recruiting impacts on-field performance in college football, based on recruiting ranking and points, to quantify the impact it has on differences
between winning and losing.

## How I addressed problem statement

### Data

The data used on this project came from a collge football API for R that utilized the resources below.  The analysis used the following metrics, defined below:
 
  Season Data 
  1) Team - College football teams from the five major football conferences (ACC, Big Ten, Big 12, Pac 12, and SEC)
  2) Wins - Total Wins by the team during the 2019 season.
  3) Five Year Average Recruiting Points - Average recruiting points (as determined by year by collegefootlldata.com) across last 5 recruiting classes (2015-2019)

  Game Data
  1) Home Team - Team hosting the game (or determined home team on neutral site)
  2) Home Team Score - Final score of game by home team
  3) Away Team - Visit team of game
  4) Away Team Score - Final score of game by visiting team
  5) Home Team Five Year Average Recruiting Points - Average recruiting points for the home team (as determined by year by collegefootlldata.com) across last 5 recruiting classes (2015-2019)
  6) Away Team Five Year Average Recruiting Points - Average recruiting points for the away team (as determined by year by collegefootlldata.com) across last 5 recruiting classes (2015-2019)
  7) Recruiting Point Difference - Home Team Five Year Average Points - Away Team Five Year Average Points
  8) Home Team Win - flag on whether or not the home team won the game


Resources:
  1) https://github.com/meysubb/cfbscrapR
  2) https://collegefootballdata.com/

### Methodolgy

I addressed the problem statement in two ways:
  
1) First, I looked at the season win-loss totals for the 2019 season for the major college football conferences, and analyzed how
how much impact recruiting has by using a five year average recruiting points, using linear regression.

2) In addition, I wanted to see if I could  predict the game by game performance based on recruiting ranking comparisons as well. To accomplish this, I used logistic regression
to see how accurate the model would be in picking the winner of games during the 2019 season based on which teams had higher recruiting rankings. 
