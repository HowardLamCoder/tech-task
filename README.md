# Technical task for new applicants

## Requirements

The task is to create a basic web application that displays the current temperature using https://darksky.net/ using the geo-location of your browser.

Goto https://darksky.net/dev/register signup for an account to get access to an api key.

### Key business requirements

* Display the current temperature in degrees celsius
* Display the temperature based on the geolocation (note; not the IP!) of your browser
* Display a simple icon and label based on the weather information provided (eg. sunny, cloudy, rainy etc).
* The API request must be proxied via your nodejs server application ie. do not make a request from the client side directly to https://darksky.net/ for the weather information. It must go via your localhost app.

## Getting Started

* Fork this repository.
* Install nodejs on your computer https://nodejs.org/en/  (tested on version 8.11.x)
* clone the code base
* Install the dependencies `npm install`

* To start the server `npm run start:dev`
* If everything is working fine you should see:

```
2018-05-16T03:07:02.330Z - info: *******************************************************************************************
2018-05-16T03:07:02.331Z - info: * Server is running http://localhost:4000
2018-05-16T03:07:02.331Z - info: * Environment development
2018-05-16T03:07:02.331Z - info: *******************************************************************************************
```
* on your browser goto: http://localhost:4000

* Commit your code, and send us a pull request when you are finished.


### Complete each task below:
### Task 1
Using this code base, create an endpoint to proxy a request to api.darksky.net and return a
response with the current temperature for your location based on the geolocation
and display it on the homepage http://localhost:4000

Requirements:
* The MVC architectural structure is predefined for you please don't change it
* Use the scaffold to implement the missing bits of code (you will see comments through out the code base to guide you) to get the application working
* In the /src/modules/weather folder implement the models, repository, api, view and anything else
that you see fit to get the application to inject the response from the api into the template.
* Commit and push your code regularly

### Task 2
Style the template based on the image provided into html and css.
```/src/public/sample-gui.png```
Requirements:

The image of the weather should be based on the forecast:

Cloudy should display a cloud, sunny should display a sunshine and so forth

### Task 3
Coding style: https://github.com/airbnb/javascript
You will notice the code uses linting, tests and type checking

Requirements:
* Fix any linting issues based on the coding style provided
* Run ```npm run build``` should not produce any warnings or errors

### Task 4
Submit your code by making a pull request

If you have any questions please email: jay@firstever.com

