
# Open Tree Data Analysis
### Exploring hidden tree patterns with urban walks in Rome
### Project Description
As part of STARTS.EU project, **Trees in cities** is a project that focuses on cities' green spaces, specifically on urban trees and their potential effect on the life of people. There are two main datasets in the project: depersonalized human trajectories (with induced noise) and open data of trees in Rome. We analyse layered geographical data and use statistical spatial analysis. More importantly, in this project, we introduce a new measure, **Green Index**, to assess the information about the city walks.

This project tackles the issue of the integration of trees into the cityscape. It is motivated mainly by post-COVID city crisis recovery and how to keep cities greener and more suitable for people to live in.
### Hypothesis
When walking, people prefer to walk in streets with trees rather than places without trees. Unfortunately, most mobile mapping apps currently fail to suggest that experience as they are able to offer only the shortest routes. We hypothesize that based on the people’s trajectories and tree data that we have, with hard pieces of evidence, we can find that people prefer the green path over the most straightforward way when walking.
### Data
We work with two main datasets. The first one is the data for trees in Rome. The second dataset is pseudo-anonymised data for human mobility in Rome. We consider the mobility data from 196171 users, taking into account only those which can be potentially on foot. The total number of considered trips is 1 395 719 862. The mobility data was collected by a private company developing geolocation SDKs for mobile phone apps. The SDK is optimized to sample users coordinates minimizing energy consumption, hence temporal resolution may vary from a few seconds to some minutes. 

### Analysis Notebooks
Analysis notebooks includes different parts of analysis on people's trajectories and trees:
(updated by Yasamin)

* 1. [green_index_calculation](https://github.com/Liyubov/open_tree_data_analysis/blob/main/notebooks/analysis/1.%20green_index_calculation.ipynb):
    In this notebook there are all preparations of all trajectories dataset with trees dataset. Here you can find:
    * Analyzing all trajectories from "all_trajectories" file
    * Estimating distance between each two stops of a trip in "distance_km" and "distance_minutes" column
    * Estimating the number of trees around each stop in "number_trees" column
    * Defining "green_index" both in time and distance
    * Estimating clustering of mobility points
* 2. [green_index_plotting](https://github.com/Liyubov/open_tree_data_analysis/blob/main/notebooks/analysis/2.%20green_index_plotting.ipynb):
    In this notebook we use the dataset we made in previous notebook (green_index_calculation.ipynb) and plot the trajectories in city map. In this notebook we have: 
    * Discovering the correlation between distance and time at each stop
    * Scatter Plots for showing the correaltion between distance and time
    * Plotting all the trajectories in city map
    * Defining the outliers and plotting them on the map    
* 3. [centrality_measure_for_trees](https://github.com/Liyubov/open_tree_data_analysis/blob/main/notebooks/analysis/3.%20centrality_measure_trees.ipynb):
    In this notebook there are calculations for estimating the centrality betweenness and degree centrality for trees using OSMNX and Networkx.
* 4. [clustering_mobility_and_tree_data](https://github.com/Liyubov/open_tree_data_analysis/blob/main/notebooks/analysis/4.%20clustering_mobility_and_tree_data.ipynb):
    In this notebook there clustering trajectories and trees in the city map. 
* 5. [betweenness_city_streets_for_tree](https://github.com/Liyubov/open_tree_data_analysis/blob/main/notebooks/analysis/5.%20betweenness_city_streets_for_tree.ipynb):
     Some attempts for loading different parts of Rome using OSMNX (can be removed or merged with other notebooks) 
* 6. [data_mobility_analysis](https://github.com/Liyubov/open_tree_data_analysis/blob/main/notebooks/analysis/6.%20data_mobility_analysis.ipynb):
    There are some plots of different indices (can be removed or merged with other notebooks) 
* 7. [explore_full_data_rome](https://github.com/Liyubov/open_tree_data_analysis/blob/main/notebooks/analysis/7.%20explore_full_data_rome.ipynb):
    Some plots of different tree datasets on city map (can be removed or merged with other notebooks) 
* 8. [green_walk_index_mobility](https://github.com/Liyubov/open_tree_data_analysis/blob/main/notebooks/analysis/8.%20green_walk_index_mobility.ipynb):
    Calulation of green index (can be removed)

# Paper 
Our paper is accepted to the journal of Cartography (2023) special issue. 
In process of publication to be shared.

# Contributions 
From L. and Y. (LPI).


