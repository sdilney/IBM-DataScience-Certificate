# IBM-Capstone-Certificate
To develop the model the data will be focused on accidents that occurred between 05:00am and 09:00am each morning. In addition to the severity code, the data that references ambient conditions and locations will be utilized to develop the 2-step model for the user. The geographic data will be used to map the most likely area of accidents that are on the commuter routes and the condition data will then be able to provide a predictor score for the user to provide them insights as to their risk of commuting. These two factors can then be used in a practical way to determine if commuting is high risk and they should decide to work from home. 

after sorting the data for the time frame of 05:00 to 09:00 the weather/situation specific conditions were extracted. These consisted for the X&Y coordinates, the address type, weather description, road condition, and light condition. The total nubmer of rowas between 05:00am and 09:00am were 18,027.

	SEVERITYCODE	X	Y	ADDRTYPE	WEATHER	ROADCOND	LIGHTCOND

The Weather, ROADCOND, and LIGHTCOND were further analyzed and simplfied to reduce the categories. For example, ROADCOND was reduced to 4 main categories.  All of this preprocessing was done before assigning dumy variables to the categories.


Dry               11601
Wet                5940
IceSnowSlush        450
SandMudDirtOil       17

