# Remote-ly

Remote-ly is an application designed for travelers looking to plan a trip to state parks around the country. Start a new trip and choose a park based on the description and plan accordingly based on local weather data for that park's area. After choosing your park you may then add restaurants and other attractions to your trip to visit along the way. You can view your saved trips and even pull up directions for your trip that navigates you to the restaurants, activities, and finally the park you are visiting.

This application was designed by me (Jon) and 3 other apprentice programmers at Nashville Software School. We utilized GitHub workflow and pair programming to plan, design, and build the application in a mock 1 and a half week sprint.

## Running the App Locally

1. Clone repo to your machine
2. Inside the main directory create a Settings.js file using the following code:
``` bash
touch Settings.js
```
3. Open up Visual Studio Code using `code .` and paste this code into the Settings.js file:
``` bash
export const keys = {
	graphhopperKey: "99bfd6c1-cba2-4ace-a1f6-cf325780242d",
	npsKey: "pi8adwTsUtwISb1FxKz1LC2BFesIOtPtORUehzk5",
	weatherKey: "48dd27ebf296f56c4be04fdd50e77663"
}
```
4. If you do not have json server installed you will need to install it using the command: 
``` bash
npm install -g json-server
```
5. In one terminal CD to api directory inside the main directory and run JSON server to port 3000 using command: 
``` bash 
json-server -p 3000 -w database.json
```
6. In another terminal window CD to the main directory and begin application using the command: 
``` bash 
serve
```

## Technologies 
* HTML
* CSS
* Javascript
* JSON Server

## External API's + Data

* National Park Service (national park api): https://www.nps.gov/subjects/digital/nps-data-api.htm
* Open Weather Map (weather api): https://openweathermap.org/api
* Graphhopper (direction api): https://www.graphhopper.com/
* Activities Data (dummy data): http://holidayroad.nss.team/bizarreries
* Restaurant Data (dummy data): http://holidayroad.nss.team/eateries

