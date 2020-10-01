# IBM-Capstone-Certificate
To develop the model the data will be focused on accidents that occurred between 05:00am and 09:00am each morning. In addition to the severity code, the data that references ambient conditions and locations will be utilized to develop the 2-step model for the user. The geographic data will be used to map the most likely area of accidents that are on the commuter routes and the condition data will then be able to provide a predictor score for the user to provide them insights as to their risk of commuting. These two factors can then be used in a practical way to determine if commuting is high risk and they should decide to work from home. 

after sorting the data for the time frame of 05:00 to 09:00 the weather/situation specific conditions were extracted. These consisted for the X&Y coordinates, the address type, weather description, road condition, and light condition. The total number of rows between 05:00am and 09:00am were 18,027.

The Main Columns used in this analysis include:

SEVERITY CODE - Either a 1 or 2 depending upoon property damage or injury respectively.  Althought the codes could include a 0,1,2, or 3, the data set seems to only be focused on the choices of 1 or 2. These will be used as the binary choice dependent variable for the analysis.

X - The lattitude coordinate of the accident. This data will be included to see if location creates additional weighting.

Y - The longitude coordinate of the accident. This data will be included to see if location creates additional weighting.

ADDRTYPE - This has a description of Block or Intersection. An intersection accidnet may indicate a perpendicular interaction wiht another vehicle or feature vs. a block that may be a more parallel interaction.

WEATHER - There are multiple descriptions of weaterh conditions in the data set.  The main factors that seem to increase severity are icy and wet conditions as expected.

ROADCOND - The road conditions are somewhat coorelated with WEATHER.  Conditions of Wet or icy are a function of the exterior conditions.  

LIGHTCOND - This is mainly a function of the time of day; however, there are different codes related to dusk, dawn, and if the streetlamps have been illuminated. In addition, some errors were found where Dusk was selected during morning hours that will need correction.

The WEATHER, ROADCOND, and LIGHTCOND were further analyzed and simplfied to reduce the categories. For example, ROADCOND was reduced to 4 main categories.  All of this preprocessing was done before assigning dumy variables to the categories.

Dry			11601
Wet			5940
IceSnowSlush		450
SandMudOil		17

