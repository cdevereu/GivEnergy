# GivEnergy Node-RED Integration
This Node-RED flow runs every day at 21:00 to pull the solar forecast from forecast.solar API and uses it to set the charge level, start time and end time on your GivEnergy battery, using their API.

What you'll need to add/change:
1. Your own location, solar array size, solar panel angle, solar panel azimuth into the forecast.solar URL.  Check the documentation for the Azimuth (direction) as it's not a straight forward compass heading.
2. Your own GivEnergy API key which you can get from the GivEnergy web portal
3. Your own cheap energy slot start and end times
4. Your own logic to determine forecast vs charge level.  The default values are already input.

I also run this flow as a paid service for those that don't want to, or don't have the skills to run it themselves.  Drop me an email for more details (see my GitHub profile)
