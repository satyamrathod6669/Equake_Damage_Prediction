# Equake_Damage_Prediction

EquakeDamagePred

Problem Statement

Task 1:- Prepare a complete data analysis report on the given data.

Task 2:- Create a predictive model in such a way that the objective is to predict the ordinal variable “damage_grade”. This column presents the level of damage grade affected by the earthquake.

Task3:- Suggestions to the Seismologists to avoid  earthquake event leading  to significant damage in many buildings


Dataset Link:

You will be predicting the amount of damage buildings receive during an earthquake. This is a Driven Data competition.
We’ve set up this Kaggle classroom competition so multiple teams within MDST can compete. The winning model will be used for our final submission to the Driven Data leaderboard.
From the Driven Data website:
We're trying to predict the ordinal variable damage_grade, which represents a level of damage to the building that was hit by the earthquake. There are 3 grades of the damage:
1 represents low damage
2 represents a medium amount of damage
3 represents almost complete destruction



●	Features
●	The dataset mainly consists of information on the buildings' structure and their legal ownership. Each row in the dataset represents a specific building in the region that was hit by Gorkha earthquake.
●	There are 39 columns in this dataset, where the building_id column is a unique and random identifier. The remaining 38 features are described in the section below. Categorical variables have been obfuscated random lowercase ascii characters. The appearance of the same character in distinct columns does not imply the same original value.
●	Description
●	· 	geo_level_1_id, geo_level_2_id, geo_level_3_id (type: int): geographic region in which building exists, from largest (level 1) to most specific sub-region (level 3). Possible values: level 1: 0-30, level 2: 0-1427, level 3: 0-12567.
●	· 	count_floors_pre_eq (type: int): number of floors in the building before the earthquake.
●	· 	age (type: int): age of the building in years.
●	· 	area_percentage (type: int): normalized area of the building footprint.
●	· 	height_percentage (type: int): normalized height of the building footprint.
●	· 	land_surface_condition (type: categorical): surface condition of the land where the building was built. Possible values: n, o, t.
●	· 	foundation_type (type: categorical): type of foundation used while building. Possible values: h, i, r, u, w.
●	· 	roof_type (type: categorical): type of roof used while building. Possible values: n, q, x.
●	· 	ground_floor_type (type: categorical): type of the ground floor. Possible values: f, m, v, x, z.
●	· 	other_floor_type (type: categorical): type of constructions used in higher than the ground floors (except of roof). Possible values: j, q, s, x.
●	· 	position (type: categorical): position of the building. Possible values: j, o, s, t.
●	· 	plan_configuration (type: categorical): building plan configuration. Possible values: a, c, d, f, m, n, o, q, s, u.
●	· 	has_superstructure_adobe_mud (type: binary): flag variable that indicates if the superstructure was made of Adobe/Mud.
●	· 	has_superstructure_mud_mortar_stone (type: binary): flag variable that indicates if the superstructure was made of Mud Mortar - Stone.
●	· 	has_superstructure_stone_flag (type: binary): flag variable that indicates if the superstructure was made of Stone.
●	· 	has_superstructure_cement_mortar_stone (type: binary): flag variable that indicates if the superstructure was made of Cement Mortar - Stone.
●	· 	has_superstructure_mud_mortar_brick (type: binary): flag variable that indicates if the superstructure was made of Mud Mortar - Brick.
●	· 	has_superstructure_cement_mortar_brick (type: binary): flag variable that indicates if the superstructure was made of Cement Mortar - Brick.
●	· 	has_superstructure_timber (type: binary): flag variable that indicates if the superstructure was made of Timber.
●	· 	has_superstructure_bamboo (type: binary): flag variable that indicates if the superstructure was made of Bamboo.
●	· 	has_superstructure_rc_non_engineered (type: binary): flag variable that indicates if the superstructure was made of non-engineered reinforced concrete.
●	· 	has_superstructure_rc_engineered (type: binary): flag variable that indicates if the superstructure was made of engineered reinforced concrete.
●	· 	has_superstructure_other (type: binary): flag variable that indicates if the superstructure was made of any other material.
●	· 	legal_ownership_status (type: categorical): legal ownership status of the land where building was built. Possible values: a, r, v, w.
●	· 	count_families (type: int): number of families that live in the building.
●	· 	has_secondary_use (type: binary): flag variable that indicates if the building was used for any secondary purpose.
●	· 	has_secondary_use_agriculture (type: binary): flag variable that indicates if the building was used for agricultural purposes.
●	· 	has_secondary_use_hotel (type: binary): flag variable that indicates if the building was used as a hotel.
●	· 	has_secondary_use_rental (type: binary): flag variable that indicates if the building was used for rental purposes.
●	· 	has_secondary_use_institution (type: binary): flag variable that indicates if the building was used as a location of any institution.
●	· 	has_secondary_use_school (type: binary): flag variable that indicates if the building was used as a school.
●	· 	has_secondary_use_industry (type: binary): flag variable that indicates if the building was used for industrial purposes.
●	· 	has_secondary_use_health_post (type: binary): flag variable that indicates if the building was used as a health post.
●	· 	has_secondary_use_gov_office (type: binary): flag variable that indicates if the building was used fas a government office.
●	· 	has_secondary_use_use_police (type: binary): flag variable that indicates if the building was used as a police station.
●	·     has_secondary_use_other (type: binary): flag variable that indicates if the building was secondarily used for other purposes.


Overview
Based on aspects of building location and construction, your goal is to predict the level of damage to buildings caused by the 2015 Gorkha earthquake in Nepal.
 
This is an intermediate-level practice competition.
The data was collected through surveys by Kathmandu Living Labs and the Central Bureau of Statistics, which works under the National Planning Commission Secretariat of Nepal. This survey is one of the largest post-disaster datasets ever collected, containing valuable information on earthquake impacts, household conditions, and socio-economic-demographic statistics.

Problem description
We're trying to predict the ordinal variable damage_grade, which represents a level of damage to the building that was hit by the earthquake. There are 3 grades of the damage:
•	1 represents low damage 
•	2 represents a medium amount of damage 
•	3 represents almost complete destruction 

Features

The dataset mainly consists of information on the buildings' structure and their legal ownership. Each row in the dataset represents a specific building in the region that was hit by Gorkha earthquake.
There are 39 columns in this dataset, where the building_id column is a unique and random identifier. The remaining 38 features are described in the section below. Categorical variables have been obfuscated random lowercase ascii characters. The appearance of the same character in distinct columns does not imply the same original value.
Description
•	geo_level_1_id, geo_level_2_id, geo_level_3_id (type: int): geographic region in which building exists, from largest (level 1) to most specific sub-region (level 3). Possible values: level 1: 0-30, level 2: 0-1427, level 3: 0-12567. 
•	count_floors_pre_eq (type: int): number of floors in the building before the earthquake. 
•	age (type: int): age of the building in years. 
•	area_percentage (type: int): normalized area of the building footprint. 
•	height_percentage (type: int): normalized height of the building footprint. 
•	land_surface_condition (type: categorical): surface condition of the land where the building was built. Possible values: n, o, t. 
•	foundation_type (type: categorical): type of foundation used while building. Possible values: h, i, r, u, w. 
•	roof_type (type: categorical): type of roof used while building. Possible values: n, q, x. 
•	ground_floor_type (type: categorical): type of the ground floor. Possible values: f, m, v, x, z. 
•	other_floor_type (type: categorical): type of constructions used in higher than the ground floors (except of roof). Possible values: j, q, s, x. 
•	position (type: categorical): position of the building. Possible values: j, o, s, t. 
•	plan_configuration (type: categorical): building plan configuration. Possible values: a, c, d, f, m, n, o, q, s, u. 
•	has_superstructure_adobe_mud (type: binary): flag variable that indicates if the superstructure was made of Adobe/Mud. 
•	has_superstructure_mud_mortar_stone (type: binary): flag variable that indicates if the superstructure was made of Mud Mortar - Stone. 
•	has_superstructure_stone_flag (type: binary): flag variable that indicates if the superstructure was made of Stone. 
•	has_superstructure_cement_mortar_stone (type: binary): flag variable that indicates if the superstructure was made of Cement Mortar - Stone. 
•	has_superstructure_mud_mortar_brick (type: binary): flag variable that indicates if the superstructure was made of Mud Mortar - Brick. 
•	has_superstructure_cement_mortar_brick (type: binary): flag variable that indicates if the superstructure was made of Cement Mortar - Brick. 
•	has_superstructure_timber (type: binary): flag variable that indicates if the superstructure was made of Timber. 
•	has_superstructure_bamboo (type: binary): flag variable that indicates if the superstructure was made of Bamboo. 
•	has_superstructure_rc_non_engineered (type: binary): flag variable that indicates if the superstructure was made of non-engineered reinforced concrete. 
•	has_superstructure_rc_engineered (type: binary): flag variable that indicates if the superstructure was made of engineered reinforced concrete. 
•	has_superstructure_other (type: binary): flag variable that indicates if the superstructure was made of any other material. 
•	legal_ownership_status (type: categorical): legal ownership status of the land where building was built. Possible values: a, r, v, w. 
•	count_families (type: int): number of families that live in the building. 
•	has_secondary_use (type: binary): flag variable that indicates if the building was used for any secondary purpose. 
•	has_secondary_use_agriculture (type: binary): flag variable that indicates if the building was used for agricultural purposes. 
•	has_secondary_use_hotel (type: binary): flag variable that indicates if the building was used as a hotel. 
•	has_secondary_use_rental (type: binary): flag variable that indicates if the building was used for rental purposes. 
•	has_secondary_use_institution (type: binary): flag variable that indicates if the building was used as a location of any institution. 
•	has_secondary_use_school (type: binary): flag variable that indicates if the building was used as a school. 
•	has_secondary_use_industry (type: binary): flag variable that indicates if the building was used for industrial purposes. 
•	has_secondary_use_health_post (type: binary): flag variable that indicates if the building was used as a health post. 
•	has_secondary_use_gov_office (type: binary): flag variable that indicates if the building was used fas a government office. 
•	has_secondary_use_use_police (type: binary): flag variable that indicates if the building was used as a police station. 
•	has_secondary_use_other (type: binary): flag variable that indicates if the building was secondarily used for other purposes. 
 
Feature data example

Here's an example of one of the rows in the dataset so that you can see the kinds of values you might expect in the dataset. Some are numeric, some are categorical, and there are often missing values. 
field	value
geo_level_1_id	8
geo_level_2_id	396
geo_level_3_id	1108
count_floors_pre_eq	2
age	15
area_percentage	4
height_percentage	7
land_surface_condition	t
foundation_type	r
roof_type	n
ground_floor_type	v
other_floor_type	q
position	s
plan_configuration	d
has_superstructure_adobe_mud	1
has_superstructure_mud_mortar_stone	1
has_superstructure_stone_flag	0
has_superstructure_cement_mortar_stone	0
has_superstructure_mud_mortar_brick	0
has_superstructure_cement_mortar_brick	1
has_superstructure_timber	0
has_superstructure_bamboo	0
has_superstructure_rc_non_engineered	0
has_superstructure_rc_engineered	0
has_superstructure_other	1
legal_ownership_status	v
count_families	1
has_secondary_use	0
has_secondary_use_agriculture	0
has_secondary_use_hotel	0
has_secondary_use_rental	0
has_secondary_use_institution	0
has_secondary_use_school	0
has_secondary_use_industry	0
has_secondary_use_health_post	0
has_secondary_use_gov_office	0
has_secondary_use_use_police	0
has_secondary_use_other	0

