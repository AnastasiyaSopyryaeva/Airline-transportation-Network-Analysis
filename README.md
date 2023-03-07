# Airline-transportation-Network-Analysis

The study is conducted as as an end-of-course project for the "Network Analysis" course of the Master Degree in Digital Humanities and Digital Knowledge of the University of Bologna, held by professor Giallorenzo Saverio.

The purpose of the project is to conduct network study in the field of spatial networks. In particular, I conducted a comparative study of airline passenger transportation networks of Russia (inside/to/from the country) in two different time spans: before and after international sanctions of 2014-2022. The main idea is to discover differences that occurred after the sanctions have been applied.



## Resources and tecchnologies used for the project

### Datasets
The data for the project was found online on various open web resources: 
- Flight route data between world airports was found as datasets with tabular data on Airline Route Mapper (http://arm.64hosts.com). 
- The list of IATA codes for Russian airports was retrieved from Wikipedia (https://en.wikipedia.org/wiki/List_of_airports_in_Russia) and stored as .csv. 
- Dataset with tabular data on the geographic coordinates of airports was downloaded from OurAirports (https://ourairports.com/data/) and stored as .csv. 

### Tools
As a tool for data manipulation, visualisation and analysis I chose Jupyter Notebook platform and various Python libraries, mainly: 
-	Pandas, in order to read .tsv or .csv datasets and convert them to Python-friendly dataframes;
-	NetworkX, main python library for network analysis which allows to draw graphs and compute their measures;
-	Cartopy, in order to enable geographic representation.

### Measures
- General descriptive statistics of the networks;
- Average shortest path length / closeness centrality (measuring the mean distance from a node to all the other nodes);
- Degree centrality distribution (shows the number of connections to a node);
- Betweenness centrality distribution (shows the extent to which a node lies on paths between other nodes);
- K-cores (k-core is a connected set of nodes where each is joined to at least k of the others);
- K-components (k-component is a set of nodes such that each is reachable from each of the others by at least k node-independent paths);
- Clustering coefficient of the networks (the likelihood of the neighbours of a node of being neighbours as well);
- Connectivity, beta index (dividing the total number of arcs in a network by the total number of nodes).
