# Project 
### Title
	Weather
### Created by
	Joostens Tomek
### Description
	This module helps you to interface with the openweathermap API
### Version
	1.0.1


# Setup
	python setup.py install


# Retrieve API
### 1. Create an account on openweathermap website
	https://home.openweathermap.org/users/sign_up
### 2. Get your API key
	https://home.openweathermap.org/api_keys

### 3. Create config file in the folder listed in the root folder
	Config/config.ini
### 4. Add following lines to the config file
	[Openweathermap]
	API = INSERT_API_KEY_HERE


# Example
### Import module
	import Weather
### Create object, first parameter is the place you want to fetch the weather from
	w = Weather.Weather('Tokyo')
### Optionally add as the second parameter the absolute path to the config file
	w = Weather('Tokyo','C://path/to/config.ini')
### Print temperature in metric units
	print(w.temperature)
### Print minimum temperature in metric units
	print(w.min_temperature)
### Print maximum temperature in metric units
	print(w.max_temperature)
### Print humidity in metric units
	print(w.humidity)
### Print weather description
	print(w.description)
### Print detailed weather description
	print(w.detailed)


