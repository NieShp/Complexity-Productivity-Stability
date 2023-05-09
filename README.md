# Complexity-Productivity-Stability
Dataset of empirical food webs and Matlab code in the paper "Will a large complex system be productive?" (published in Ecology Letters).

This ZIP file have two subploder. 

## Description of the data and file structure: 

In the folder "empirical_data", 3 files are list:

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

## Sharing/Access information

The dataset of empirical food webs can be obtained from each published study/reference listed in the file “Overview_of_149_food_webs.xlsx”. Those studies have built the Ecoptah model. However, the dataset of empirical food webs is also available from EcoBase: http://ecobase.ecopath.org/. See the methods in our paper. 
