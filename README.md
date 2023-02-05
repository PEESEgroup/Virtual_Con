# Trend of virtual and hybrid conferences since COVID-19 effectively mitigate climate change
We investigated the potential of switching in-person conferences to virtual or hybrid mode in reducing environmental impacts. 
## Scenarios
The three Excel files contains all modeling parameters and input data for the studied conference scenarios based on ACLCA virtual conference in 2020. The virtual scenario is the baseline. The in-person scenarios models in-person conferences with 1 to 6 hubs. Two sets of hybrid scenarios with different constraints are considered to investigate the trade-offs between in-person interactions and the environment impact of hybrid conferences, as described in the following: 
-	 “maximum travel distance” scenarios:  the maximum one-way travel distance (1,000 km, 3,000 km, 5,000 km, or 10,000 km), and the number of conference hubs.
-	 “maximum virtual participation” scenarios: the maximum virtual participation level (10%, 30%, 50%, or 70%) and the number of conference hubs.

Each set of hybrid scenarios involves 1 to 6 hubs. The locations of conference hubs for each scenario are determined using the facility location optimization model for shortest total travel distances. Moreover, the facility location optimization model also makes decisions for participants on whether they attend virtually or which hub should they go.
## Data Files
The first tab of each Excel file is named "outline", which lists the content of each tab.
### Catering.xlsm: 
This file contains LCI and LCIA for the catering stage of conferences.
### Virtual Con_Hybrid.xlsm: 
This file contains LCI and LCIA for the hybrid scenarios.
### Virtual Con_In-person&Virtual.xlsm: 
This file contains LCI and LCIA for the in-person and virtual scenarios.
## Code files
Code for looking for the nearest airport of each participant, calculating total travel distance, and optimization model are provided in this file. The imported and exported files are also available.
### Participant nearest airport
This file looks for the nearest airport of each participant. "Geocoordinate.csv" and "World60_US60_airport.csv" are imported and "Participant_nearest_airport.csv" are exported.
### Distance computing
This file computes the total travel distance for each participant. "Geocoordinate.csv", "Alternative hub locations.csv", and "Participant_nearest_airport.csv" are imported and "Distance_matrix_1hub.csv" and "Distance_matrix_multihub.csv" are exported.
### Optimization model
This file executes the optimization model to look for optimal hubs and participant assignments to these hubs. "Distance_matrix_1hub.csv" and "Distance_matrix_multihub.csv" are imported and "df_result_final" are generated. 
## Citation
Please use the following citation when using the data, methods or results of this work:
> Tao, Y., Steckel, D., Klemeš, J.J. et al. Trend towards virtual and hybrid conferences may be an effective climate change mitigation strategy. _Nature Communications_ 12, 7324 (2021). https://doi.org/10.1038/s41467-021-27251-2
> 
> [![DOI](https://zenodo.org/badge/407425669.svg)](https://zenodo.org/badge/latestdoi/407425669)
