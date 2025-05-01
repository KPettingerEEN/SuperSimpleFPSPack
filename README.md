# The Super Simple FPS Pack

__This pack was made from the orginal First Person Shooter template for Unreal Engine 5.5 and has been updated to include:__

* A fresh weapon *(M4)* with animations rigged and made with blender and a preset animation blueprint
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
* You can either follow the steps below to create a new level blueprint OR migrate the content folder using the instructions later on

_____________________________________________________________________________________________

__Creating a New Level Blueprint:__

* Open up the Character folder
* Create a new level blueprint
* Name it what you want
* Add the following objects to the world:
  
  1. SkyLight
  2. Sky Atmosphere
  3. Directional Light
  4. Volumetric Clouds
  5. Player Start
 
* Then you will need to add a landscape or a plane to the level and adjust the player start to be level with the ground
* Once the level is saved, go to your "Project Settings"
* In the project settings, navigate under "Project" and look for "Maps & Modes"
* Change the Startup Map and Default Map to the new level you created
* The game mode and character should already be set
* Restart the project
* Click "Play" and happy building!

_____________________________________________________________________________________________

__Migrating the Content Folder:__

* Highlight the "Content" folder by left clicking on it
* Right click the Content folder and select "Migrate"
* In the migration menu, ensure that ALL contents of the Character and Demo folder are selected (besides the level)
* After you confirm, you will have to find the project folder for the project you want to migrate to within your computer storage
* You must select the "Content" folder for the project in order for the migration to work
* Once complete close out of the project and open the project you migrated to and you will see the new folder with all of the contents
* Navigate to the Project Settings
* Under "Project" look for "Maps & Modes"
* Change the default game mode to "GM_FPS"
* Click play and enjoy!

*If you run into any issues with migration, it is most likely that the animation blueprint is broken. To fix it you just need to reconnect the corresponding animation sequences to their states within the state machine. This shouldn't happen but sometimes when migrating a project the custom names change, which can cause the links to quite literally break. Typically this happens with Custom Event nodes, Animation Sequences, and variables that are specific to certain actor or class references.*

_____________________________________________________________________________________________

__Note:__ If you happen to run into any issues please join my discord here and reach out to me - https://discord.gg/BbDVRMJ2V7
