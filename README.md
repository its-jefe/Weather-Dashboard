# 06 Server-Side APIs: Weather Dashboard

Deployed @ https://its-jefe.github.io/Weather-Dashboard/

This is [project #6][1] for [UCF Coding Bootcamp][2]

---

Uses the [OpenWeather One Call API](https://openweathermap.org/api/one-call-api) along with the [OpenWeather Current Weather Data API](https://openweathermap.org/current) to retrieve weather data for cities. 

## Usage
- Users may enter a city into the search field and hit search. They are then able to view the current conditions and 5-day forecast for that city. (with matching weather icons 😲)
- The searched cities are saved in a list and can be revisted.
- If the city is typed incorrectly or is not found in the database, an alert window will show and inform the user. 

## Implementing 
- `JavaScript`, `CSS`, `HTML`
- 2 OpenWeather `APIs`
- `localstorage`
- Error handling


[1]: https://github.com/UCF-Coding-Boot-Camp/UCF-VIRT-BO-FSF-PT-04-2021-U-B/tree/main/06-Server-Side-APIs/02-Challenge
[2]: https://bootcamp.ce.ucf.edu/coding/

## Future Implementation
- I enjoyed this as a learning module but don't see working on it any further.

## Needs Fix
> There is a small bug regarding the date. As I write this note I'm sitting in the central US timezone. The current date is 6/08/21 yet when I query ‘Funafuti’, the app still displays 'Tue Jun 08' even though the current date in Funafuti is 6/09/21. 
>> Use the `timezone_offset` key from the one call API response to generate and display the correct date for the queried location. This key is an integer (positive or negative) representing the number of seconds the queried location is offset from unix time. 
