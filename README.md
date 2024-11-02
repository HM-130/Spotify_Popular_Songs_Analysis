# Spotify Popular Songs Analysis
*(Completed at age 14 - November 2024)*

## Overview
This is a smaller, practice project. Conducted an overview of characteristics of the hit songs in the UK for 2024, and the hit songs of the 1970s (50 year gap). 
The goal was to find the characteristics that most popular songs have, and observe how the most popular music has changed over the last 50 years.

## Project Motivation
I did this project because my favourite thing other than nerdy computer stuff is music, and this allowed me to somewhat combine the two.
It also allowed me to develop my data handling and analysis skills further.

## Data Gathering
I used the spotify web API to gather this data. I created a spotify for developers account, and made two apps which allowed me to import the data into my program. This involved finding spotify playlists that included the top ___ songs of 2024 (current day) and 50 years ago (1970 ish). I found the playlist IDs by copying the link. I prefer having a csv file with my data in, so converted the table to csv format.

## Enviroment used
Python with pandas, matplotlib, and spotipy libraries used with a Jupyter Notebook and VSCode. I analysed both datasets in one notebook.

## Histograms
After calling .describe() to gather general statistics, I used matplotlib's 'pyplot' to plot histograms of each of the 4 characteristics each song had - danceability, energy, valence, and loudness. I repeated this process for the 1970s hits, after plotting 2024's values. This gave a good idea of qualities of hit songs. 

## Bar Charts
The final step was plotting bar charts of mean values. I found the mean value of each column within the 2 datasets. I then plotted 4 bar charts of the values from each timeframe against eachother. This was very useful for visualising how the most popular music has changed.

## Findings
I concluded that hits in 2024 are on average: more danceable (with the mean value increasing by 0.04), more energetic (with the mean value increasing by roughly 0.1), have lower valence (with the mean value decreasing by roughly 0.1), and are louder (with the mean decibels increasing by roughly 4), than hits in the 1970s. Please keep in mind that this is just a project that I did to practice my skills. It doesn't take into account events happening in these time periods, and the playlists themselves might be indeed inaccurate. Please take into account the different amounts of songs in each csv, they were the best playlists I could find on spotify.

## Project Files
- [Analysis Notebook](analysis.ipynb) - Main analysis performed on the data 
- [2024 top 50 songs](spotify_top_2024.csv) - The top 50 hits in 2024
- [1970 top 100 songs](spotify_top_1970.csv) - The top 100 hits in the 1970s
