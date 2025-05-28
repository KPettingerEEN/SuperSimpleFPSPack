# The Super Simple FPS Pack

__This pack was made from the orginal First Person Shooter template for Unreal Engine 5.5 and has been updated to include:__

* An M4 and Pistol - Both Modular and already animated
* A holographic sight with two different reticles
* 8 Different Weapon Camo Materials
* A HUD with a Minimap
* A Settings menu (Fully Funtional)
* Shooter AI with Cover Finding Logic

# Instructional

* Most instructions for using the package are included within their corresponding blueprint event graphs in the form of comments.

__Getting Started:__

* You will notice that I included a video for setting up a basic game with the pack. This video is still relevant and will work even with the updates to the pack. So if you wanted to get started with a free character model and environment pack, make sure you check out that video!
* Please note that the video uses UE 5.5 assets, and you will need to be on that version to use those packs together. If you want to use this with say a 5.4 metahuman, it will still work. However, the free Character Model and Environment were not built by me so I can't tell you if they work on an earlier engine version or not.
* I suggest replacing existing buildings by building your own, because the "Stairs" in the Environment pack are not properly angled for Unreal Engine default incline mechanics. If the building does not have any stairs then it really isn't an issue.
* After you get everything from the video set up, you need to place "Cover Points" and "AI Spawns" on the map for your AI.
* Below I included instructions for migration in the event that you would like to migrate my project or any parts of it into an existing project of your own.

_____________________________________________________________________________________________

__Controls:__

Most of the controls are standard for any FPS but I also included controls for switiching between the holographic and ironsights, as well as switching between 3 weapon skins so you can see how it works, those controls are:

* Camo 1: Keyboard Number 1
* Camo 2: Keyboard Number 2
* Camo 3: Keyboard Number 3
* Change Sights: Keyboard Number 4
* Change Reticle: Left Alt
* To open the Pause Menu: Escape
* To open the Settings Menu: Click the Controller Icon in the Pause Menu
* To load a Saved Game: Click Continue in the Pause Menu

Note: If you want to use other camos, the logic is already there and there are 6 other weapon camos for you to test out. If you want to create a menu for changing camos, you can quite literally use the logic I already set up, you just need to set up bottons to call the events to change the camo to the desired one.

_____________________________________________________________________________________________

__Fixing Issues:__

1. There is an issue with the "Projectiles" that can be fixed using the steps below:

* Open a Projectile blueprint
* Click on the Projectile Movement object
* Change the Initial and Max speed of the projectile to 10000
* Change the Velocity to 10000
* Change the "Gravity" to .1 to simulate a slight bullet drop, without messing up the offset of the projectile
* Finally, click on the "Capsule" object, and change the Scale to .01


2. There is an issue with the Projectile Spawning logic for the M4 due to the above issue, and can be resolved using the steps below:

* Open the BP_M4_Modular actor blueprint in the Weapons/M4 folder
* Delete the arrow from the M4 that is located near the iron sight
* Then hop over to the BP_Player blueprint
* Change the projectile spawning logic to use the muzzle arrow instead
* This will fix any projectile issues that you may have, including close range hit registration issues.

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
