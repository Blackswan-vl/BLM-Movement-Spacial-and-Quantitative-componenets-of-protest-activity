# BLM-protests

The dataset that is utilized in this study, is based on the data provided by Crowd Counting Consortium. Specifically, data on the average number of protesters, geographic location (latitude and longitude), information source (HTML links for the new articles/twits describing the event) were extracted for further creation of the dataset variables. The state violence and protesters violence exposure were coded manually in respect to the information source.
 	In order to create codes for the violence exposure by protesters and violence exposure by the state, all the information sources were carefully investigated, applying the following coding system to create the previously mentioned variables: 1- for the cases of violence exposure and 0 otherwise (see the detailed description below). The data on geographic location was exploited for the calculation of distance from the centre of the protest hot spot to the city centre using the Manhattan distance measure since most of the cities in the United States are constructed in accordance with the block system. This measure allows calculating how many squares in a grid (or blocks in a city) we would have to go through to get from point A (protest’s hotspot) to point B (the center of the city) using the following formula (Apparicio et.al. 2003):
                                                                                    
                                                                                    |x1-x2|+|y1-y2|                                                                 
                                                           
Other explanatory variables were created using the data from the US government official website, mainly, the size of the city, number of police officers per state, the proportion of the black population in the state. 
Therefore, the dataset utilized in this study includes the following variables:

Independent variables:
1.	Distance (continuous): the Manhattan distance from the centre of the hotspot to the city centre;
2.	Size mean (continuous): the average number of people who participated in the protests.

Control variables:
1.	Large (dichotomous): 1 if the city is large (defined by two parameters - population and area), 0- if the city is small;
2.	Pol ratio (continuous) - the rate of full-time law enforcement employees per 1,000 inhabitants;
3.	BlackTotalPerc (continuous) - the proportion of black population in relation to the overall population of the state;
4.	Violence_protesters (dichotomous):1 for violence exposure (injuries, use of chemical agents cause to police), 0 - peaceful protest.

The dependent variable:
1.	State violence (dichotomous): 1 for violence exposure (arrests, injuries, use of chemical agents, traffic control caused by police), 0 - peaceful, non-violent protest.
