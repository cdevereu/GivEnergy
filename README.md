# GivEnergy Node-RED Integration
This Node-RED flow runs every day at 21:00 to pull the solar forecast from forecast.solar API and uses it to set the charge level, start time and end time on your GivEnergy battery, using their API.

The logic here is that if it's going to be sunny tomorrow, I don't need to charge the battery as much because I want to take advantage of my free solar PV to charge the battery.  If it's going to be a dull day, charge the battery up from grid so that the house can run the following day on cheap rate electricity.

What you'll need to add/change:
1. Your own location, solar array size, solar panel angle, solar panel azimuth into the forecast.solar URL.  Check the documentation for the Azimuth (direction) as it's not a straight forward compass heading.
2. Your own GivEnergy API key which you can get from the GivEnergy web portal
3. Your own cheap energy slot start and end times
4. Your own logic to determine forecast vs charge level.  My default values are already input.

I also run this flow as a paid service for those that don't want to, or don't have the skills/hardware to run it themselves.  Drop me an email for more details (see my GitHub profile)

* Copy the json file contents and IMPORT into Node-RED > Burger Menu > Import > Ctl-V
