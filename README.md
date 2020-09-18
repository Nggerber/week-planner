
Project overview

The goal of this project was to create a schedule for a typical work day. The goal was for the app to display the current time and day and then a series of time blocks for 
each hour of the work day 9am to 5pm. I am used to using a 24 hour clock and saw some instances where it might make this assignment easier so I opted for 9:00 to 17:00. The 
app is supposed to allow for some one to enter tasks into each of the time blocks and save those tasks so they could reference them later. The text was also supposed to stay in place even if the page is refreshed. Also as the time of the day progressed the color of the text blocks was supposed to change based on if the event was in the past present or future.

HTML

I used bootstrap grid system and the classes provided in the css document to create 9 different rows. Each with their own save button input field for text and element that shows which hour it is. It was also important that that I added unique id's to the seperate save buttons and input fields so that I could differentiate between them when I needed to tell which tasks were in each block.

Script

I started off my script using .moment to get the current day and time and I formatted it with capital H so the time would be displayed in a 24 hour clock I then displayed this in the header of the page. I then made variables that corresponded to each different input field. In order to save the users input I created a click function for when you hit a save button. Since each button has a seperate Id I was able to focus on that attribute and bull it out of each individual click. It then selects the specific text field to save in local storage. This values are then reloaded when the page is opened again and refreshed. Next I had to create a function that checked the current time and compared it to the values on the individual blocks. I used .moment to get the specific hour and then ran though the specific data id attached to each input field to to get the hour for that block. I then used a if else statement to compare those values to see if the fell in the past present or future and assigned them the proper class.

![day-planner](https://user-images.githubusercontent.com/67764086/93631013-25aae480-f9a8-11ea-8622-816ce7478d1c.PNG)

