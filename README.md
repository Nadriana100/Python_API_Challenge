# Python_API_Challenge
Working with APIs
Summary by Norma Espinosa
Weather Py 
Using Open Weather Map API was our main tool to find the main reason of this homework. That was to find the best place to have vacations and the hotel name, using Google Places API. 
Finding countries that are close to the Equator, getting the best weather conditions we could get our maps, locations, and name of the hotels. 
Before to start the summary of my homework, I would like to mention that hiding the Google maps password was extraordinary. I enjoyed extremally this homework, it took me a lot of hours, but I learned a lot, and this homework has helped me as a reference. This homework was the AHHH! moment when all you have learned started making sense. Probably I am exaggerating, because at the end of each homework I have had the AAAHHHHH! moment. It just because the maps amazed me. 
Ok, here I go….
As you know the cities that are closer from the equator are warmer places, but that doesn’t mean that all of them are the best places to have a warm enjoyable vacation. For that reason, we are going to use Open Weather Map API, to find the better weather conditions. 
Latitude is a fundamental control on every climate. It affects temperature by influencing the seasonal range in solar intensity. It influences precipitation in as much as evaporation is temperature dependent.
In geography, latitude is a geographic coordinate that specifies the north–south position of a point on the Earth's surface. Latitude is an angle (defined below) which ranges from 0° at the Equator to 90° (North or South) at the poles. Lines of constant latitude, or parallels, run east–west as circles parallel to the equator. Latitude is used together with longitude to specify the precise location of features on the surface of the Earth. On its own, the term latitude should be taken to be the geodetic latitude as defined below. Briefly, geodetic latitude at a point is the angle formed by the vector perpendicular (or normal) to the ellipsoidal surface from that point, and the equatorial plane. Also defined are six auxiliary latitudes that are used in special applications.





Steps to get the best weather analysis: 
1. Dependencies: matplolib, pandas, numpy, scipy.stats, your api_key, citipy, and csv.file.
2. Using the Latitude and longitude easy peace way to know the places that are close to the equator.
3. Getting my query_url using the imperial units, since temperature is set in Fahrenheit unit, checked in the cvs file. I had a problem because I used the time.sleep(60), it took more than 24 hours to list all cities (as recommendation, DO NOT USE 60).
4. Using dictionaries we convert the raw data into Data Frame, and also save it into cvs to be used that data for the Vacation Py part.
5. After this filtering the data is where we start getting the best places, 1st we knew that were not places with more than 100% of humidity.
6. Got the mean of Cloudiness, Humidity, Latitude, Longitude, Max Temperature, Min Temperature, and Wind speed. 
7. Cleaning the data, ready to plot.

8. Latitude Analysis: 

Temperature vs. Latitude 
Temperature is inversely related to latitude. As latitude increases, the temperature falls, and vice versa. Generally, around the world, it gets warmer towards the equator and cooler towards the poles
Latitude vs Humidity 
Relative humidity changes when temperatures change. Because warm air can hold more water vapor than cool air, relative humidity falls when the temperature rises if no moisture is added to the air




Latitude vs Cloudiness
As this warm, moist air rises and cools at higher altitudes, it loses its capacity to hold water vapour which condenses into clouds producing regular thunderstorms.
The cold dry air then sinks back to the surface at about 30 degrees latitude.
Clouds also commonly form in the middle latitudes 60 degrees north and south of the equator where polar and mid-latitude Ferrel circulation cells collide, which pushes air upwards, fuelling the formation of large-scale frontal systems that dominate weather patterns.
Ferrel cells are an atmospheric eddy formed by the upward movement of polar air currents at about 60 degrees latitude and the downward flow of cool dry air from the Hadley cycle at about 30 degrees latitude.

Latitude vs Wind Speed 

Since the atmosphere is fixed to the earth by gravity and rotates with the earth, there would be no circulation if some force did not upset the atmosphere's equilibrium.  The heating of the earth's surface by the sun is the force responsible for creating the circulation that does exist.
Because of the curvature of the earth, the most direct rays of the sun strike the earth in the vicinity of the equator resulting in the greatest concentration of heat, the largest possible amount of radiation, and the maximum heating of the atmosphere in this area of the earth.  At the same time, the sun's rays strike the earth at the poles at a very oblique angle, resulting in a much lower concentration of heat and much less radiation so that there is, in fact, very little heating of the atmosphere over the poles and consequently very cold temperatures.Cold air, being more dense, sinks and hot air, being less dense, rises.  Consequently, the rising warm air at the equator becomes even less dense as it rises and its pressure decreases.  An area of low pressure, therefore, exists over the equator.
Warm air rises until it reaches a certain height at which it starts to spill over into surrounding areas.  At the poles, the cold dense air sinks.  Air from the upper levels of the atmosphere flows in on top of it increasing the weight and creating an area of high pressure at the poles.
The air that rises at the equator does not flow directly to the poles. Due to the rotation of the earth, there is a build up of air at about 30° north latitude. (The same phenomenon occurs in the Southern Hemisphere).   Some of the air sinks, causing a belt of high-pressure at this latitude.
9. Linear regression Analysis 
NORTHSOUTH
Vacation Py 
10. After finding the cities that are close to the equator, we found 517 cities. 




11. Narrowing down the Data Frame to find the ideal weather condition. Of course Mexico is on the list of the 5 places around the world with the best weather conditions. 





12. Finally, you can see using Google Places API to find the 5 hotels for each city located within 5000 meters of your coordinates.









Resources:
https://www.weather.gov/source/zhu/ZHU_Training_Page/winds/Wx_Terms/Flight_Environment.htm
https://www.abc.net.au/science/articles/2015/05/12/4233502.htm?site=science/tricks#:~:text=Clouds%20also%20commonly%20form%20in,systems%20that%20dominate%20weather%20patterns.
https://www.chicagotribune.com/news/ct-xpm-2009-11-15-0910190209-story.html
https://www.worldatlas.com/articles/what-is-the-effect-of-latitude-on-temperature.html#:~:text=Temperature%20is%20inversely%20related%20to,and%20cooler%20towards%20the%20poles.
https://www.vectorstock.com/royalty-free-vector/latitude-and-longitude-diagram-educational-vector-28988043
https://en.wikipedia.org/wiki/Latitude




