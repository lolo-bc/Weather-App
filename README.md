# Weather-App
This is a simple web app that can pull information on current and upcoming weather information. The user can search for a city anywhere in the world, and return the weather data for that day as well as the next 5 upcoming days. Additionally, this app currently saves the users most recent search and repopulates the information when the page is reloaded. 

## Currently the user can return:
for current day: the date, a weather icon that represents the average weahter today, the average temperature, humidity,windspeed, and uv index
For upcoming weather: the date for the next five days, an icon that represents the weather of that day, an average of the  temperature and humidity. 

## How it works 
This app uses the API https://openweathermap.org/ to get the weather information.

When the user searches for a city name, a button is created underneath the searchbar with the same name as the search, and the weather information for that city is populated onto the page.

The user can, within the same session, click on any of those buttons, and the weather data for that city will then pop-up on the screen. 

when the user closes and re-opens the window, the last city searched for will automatically be re-created, a new button will be added, and the weather inforamtion will be on the screen. 

The user cannot search for a city + state or city + country. Currently only the city name is possible to search for. This is so that cities all around the world can be searched for 

## Future Development 
The way the city call-back function is at the moment limited. If there are several cities by the same name, the API searches for any cities with that name, and returns the first result, which may or may not be correct city the user was hoping for. In the future this app should include an elastic search wherein when the city name is typed, the various options for cities with that name, differentiated by their state and country, will pop-up as options the user can choose from. 

A dashboard where the user can save all the cities they wish to see data for in the future, instead of only the most rescent search result 

Another current limitation is that the API used to get the information for the 5 day future forecast generates 7 different icons that represents that days weather, which changes from day to night. This app pulls only the first icon and uses that to represent that day's weather. which may or may not be the most accurate representation of the day as a whole. In the future this app should find a different API to use to get more accurate repesnations of future data instead of releying on averages. 

## Built with:
https://openweathermap.org/api

