# Complexity-Productivity-Stability
Dataset of empirical food webs and Matlab code in the paper "Will a large complex system be productive?" (published in Ecology Letters).

This ZIP file has two subfolders. 

## Description of the data and file structure: 

### In the subfolder "empirical_data", 3 files are list:

empirical_data.xlsx: This file contains the detailed information and data of the 149 empirical food webs presented in our publication. For each food web, the species richness, connectance, interaction strength within and across different trophic groups (i.e., plant, herbivore and carnivore) are shown. Dimensions of this file is 150 rows by 20 columns. The descriptions of column are provided in the file "Read me for empirical_data details.txt".

Overview_of_149_food_webs.xlsx: This file gives the detailed resource of the 149 empirical food webs, including the reference, published time, latitude and longitude, etc. Dimensions of this file is 150 rows by 10 columns. The descriptions of column are also provided in the file "Read me for empirical_data details.txt".

Read_me_for_empirical_data_details.txt: the descriptions of columns in the file "empirical_data.xlsx " and “Overview_of_149_food_webs.xlsx”.

Specifically, in the file “empirical_data.xlsx”: 

  food_web:	Food webs number;

  S	:	Total speciess richness; 

  C:		Overall connectance; 

  Sigma:		Overall average interaction strength;

  Complexity:	Overall complexity measure (Sigma*sqrt(S+C));


  Stability:		Food webs stability (local stability, see Appendix S2 in our paper);

  Fun_Production:	Secondary productivity;

  C_PH	:	Connectance between plants and herbivores;

  C_PC:		Connectance between plants and carnivores;

  C_HC:		Connectance between herbivores and carnivores;

  C_CC:		Connectance links within carnivores;

  sigma_PH:	Mean interaction strength of plants on herbivores;

  sigma_PC:	Mean interaction strength of plants on carnivores;

  sigma_HC:	Mean interaction strength of herbivores on carnivores;

  sigma_CC:	Mean interaction strength within carnivores;

  S_P:  		Plants richness;

  S_H:		Herbivores richness;

  S_C:	    	Carnivores richness.

In the file “Overview_of_149_food_webs.xlsx”:

  food_web_number:		Food webs number; 

  name:			The name of the Ecopath food web; 

  country:			Country of the surveyed food web;

  type:			Food web tyle (Ecosystem tyle);

  area:			Area of the surveyed food web; 

  longtitude:			The longtitude of food web;

  latitude	:		The latitude of food web;

  year:			The time of building food webs;

  num_group:		Total speciess richness or the number of trophic groups;

  reference:			The original reference that proposed the food web;


### In the subfolder "simulated_MATLAB_code", 11 files are list:

main.m: This file is the main MATALB code for food web simulation, the recorded results (e.g., food web complexity and functioning) are saved and their meanings are provided in the file "Read me for simulated_data in code.txt".

Read me for simulated_data in code.txt: the descriptions of recorded variables in the file "main.m".

Specifically, 

In MATLAB code (allometric scaling, eqn (3), Table S1 and Appendix S2 can be seen in our study) :

  S_initial:		Initial species richness;

  C_initial:		Initial food web connectance;

  Hill.exponent:	Hill exponent (see eqn (3));

  S:	Realized food web richness;

  C:		Realized food web overall connectance;

  Sigma_partial:	Realized mean average strength (calculated form exact partial differentials, Appendix S2);

  Complexity_partial:	Overall complexity measure (calculated form exact partial differentials, Appendix S2);

  Sigma_energy	Realized mean average strength: (calculated form approximation, Appendix S2);

  Complexity_energy:	Overall complexity measure (calculated form approximation, Appendix S2);

  Biomass:		Ecosystem functioning: total biomass;

  Primary_prod:	Ecosystem functioning: primary productivity;

  Second_prod:	Ecosystem functioning: second productivity;

  S_P:		Realized plant richness;

  S_H:		Realized plant richness;

  S_C:		Realized plant richness;	

  C_PH	:	Connectance between plants and herbivores;

  C_PC	:	Connectance between plants and carnivores;

  C_HC:		Connectance between herbivores and carnivores;

  C_CC:		Connectance links within carnivores;

  sigma_PH_partial:	Mean interaction strength of plants on herbivores (calculated form exact partial differentials, Appendix S2);

  sigma_PC_partial:	Mean interaction strength of plants on carnivores (calculated form exact partial differentials, Appendix S2);

  sigma_HC_partial:	Mean interaction strength of herbivores on carnivores (calculated form exact partial differentials, Appendix S2);

  sigma_CC_partial:	Mean interaction strength within carnivores (calculated form exact partial differentials, Appendix S2);

  sigma_PH_energy:	Mean interaction strength of plants on herbivores (calculated form approximation, Appendix S2);

  sigma_PC_energy:	Mean interaction strength of plants on carnivores (calculated form approximation, Appendix S2);

  sigma_HC_energy:	Mean interaction strength of herbivores on carnivores (calculated form approximation, Appendix S2);

  sigma_CC_energy:	Mean interaction strength within carnivores (calculated form approximation, Appendix S2);

  stability_partial:	Food webs stability (calculated form exact partial differentials, Appendix S2);

  stability_energy:       Food webs stability (calculated form approximation, Appendix S2);

The other 9 file: the defined function included in the file "main.m".


## Other information
The dataset of empirical food webs is also available from EcoBase: http://ecobase.ecopath.org/. See the methods in our paper. 

## Code/Software
The file “main.m” can simulated food webs dynamics (details see our study), and the other files are the defined functions included in the file “main.m”. 

