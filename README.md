# Weather App

### Introduction:
Weather is one of the most crucial aspects of our life. It dictates the different kinds of activities that we would like to plan throughout the day, week, or month. One of the older methods of reading weather patterns is to look at the sky and predict whether it would stay sunny, rain, or have a humid weather condition.

# Weather App in Python using Tkinter module 

# Modules required:

Tkinter: It is a built-in python library for making GUI using tkinter toolkit.
Requests: It is a library which helps in fetching the data with the help of URL.

# Approach:

Firstly, we have to use a weather API for fetching the data from the Open Weather Map website by generating an API key, and then we need to create a configuration file to store the key. And finally using that configuration file in the python script.


# Steps used to create It : 

### Genterated Api key 
Login in the Open Weather Map
Go to the API section. Then in the Current Weather Data section click on the Api doc.

### Steps to create the Python script:
imported required modules 

import requests
from tkinter import *


## We have to first make the body of the GUI with the help of tkinter.

                                  app = Tk()
                                  //add title
                                  app.title("Weather App")

                                  //adjust window size
                                  app.geometry("300x300")

                                  weather_l = Label(app, text="")
                                  weather_l.pack()

                                  app.mainloop()

## Make a getweather() function to get the weather of a particular location.
                                  def getweather(city):
                                      result = requests.get(url.format(city))

                                      if result:
                                          json = result.json()
                                          city = json['name']
                                          final = [city]
                                          return final
                                      else:
                                          print("NO Content Found")

 
 ### Loading Page :
 ![image](https://user-images.githubusercontent.com/74112721/206704824-9de28c09-37e8-4a75-b4e7-7fe4c3404139.png)


# Conclusion:

Weather , plays a crucial role in our daily life. Hence, it is highly beneficial to develop a weather application that will help us track this integral element of nature successfully so that we can all plan our schedules accordingly and choose what would be the best course of action to go about in our daily life.




### About me:

This project was my first project in engineering . 

It really felt AWESome to do this Project . 

Learned About python in depth .
