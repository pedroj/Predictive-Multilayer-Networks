# Predictive-Multilayer-Networks (PMNs)
This repository contains data and R scripts accompanying McFadden and Dirzo (submitted to Nature Ecology & Evolution) Harnessing multilayer networks to predict metacommunity-wide responses to global environmental change. 

Building and analyzing a PMN
-

#### R Scripts:
- *RCode_1_Landscape_simulation.R* - contains code for simulating the starting landscape and 20 deforestation and reforestation scenarios
- *RCode_2_PMN_creation.R* - contains code for building a PMN and calculating connectance
- *RCode_3_Betweenness.R* - contains code for calculating betweenness centrality and producing figure 3
- *RCode_4_Robustness.R* - contains code for calculating multilayer robustness and producing figure 4
- *RCode_5_Fragmentation_metrics.R* - contains code for calculating a variety of forest cover and fragmentation metrics


#### Required data files for PMN creation:
-	Land cover map: *starting_landscape.tif*, or other land cover scenario of interest (created in RCode_1_Landscape_simulation.R)
-	Elevation map: *elev_map_sim.tif*
- Null network for connectance metric: *null_edge_list.csv*


#### Instructions:
The file *RCode_2_PMN_creation.R* contains a streamlines pipeline for building a PMN using the three required input files specified above. By changing the land cover input file and re-running the script, one can create additional PMNs. PMN betweenness and robustness can be calculated with RCode scripts 3 and 4. RCode script 5 contains code for calculating traditional forest fragmentation metrics, though these are provided simply for context.


#### Additional files:
- Results folder contains example outputs created by RCode scripts 2-5. Some values may not exactly match those from the paper because these data were created using separate runs of the model.


Comparing PMN structure and stability across scenarios
-

#### R Scripts:
- *RCode_6_Comparing_scenarios.R* - contains code for comparing metrics across PMNs and producing figure 5

#### Required data files:
- results csv

#### Instructions:


