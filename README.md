# The Super Simple FPS Pack

This pack was made from the orginal First Person Shooter template for Unreal Engine 5.5 and has been updated to include:

* A fresh weapon (M4) with animations rigged and made with blender and a preset animation blueprint
* Completely updated game logic from movement to projectile functionality, including ADS functionality, random recoil, custom animation states (ex. Sprinting) and more
* An easy to learn HUD
* A cleaner blueprint system with detailed notes and collapsed nodes in each event graph to make learning easy
* A data table for creating new weapons with a customizable weapon structure system
* Animation notify based events and sound cues with custom sounds for making editing easy
* Set up on the default Unreal Engine Open World map instead of the standard FPS template level for making open world game creation easier

# Instructional

* Most instructions for using the package are included within their corresponding blueprint event graphs in the form of comments.

Getting Started:

* You will notice that the default world has nothing in it, this is by design
* Open up the Character folder
* Create a new level blueprint
* Add the following objects to the world:
  
  1. SkyLight
  2. Sky Atmosphere
  3. Directional Light
  4. Volumetric Clouds
  5. Player Start
 
* Then you will need to add a landscape or a plane to the level
* Once the level is saved, go to your "Project Settings" in Unreal after you have added the package to your project of course
* In the project settings, navigate under "Project" and look for "Maps & Modes"
* Change the Startup Map and Default Map to the new level you created
* The game mode and character should already be set
* Restart the project
* Click "Play" and happy building!

Note: If you happen to run into any issues please join my discord here and reach out to me - https://discord.gg/BbDVRMJ2V7
