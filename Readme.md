
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

* betweenness_city_streets_for_tree
* data_mobility_analysis
* explore_full_data_rome
* green_walk_index_mobility
* green_index_calculation
* green_index_plotting
* centrality_measure_for_trees
* clustering_mobility_and_tree_data


