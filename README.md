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

Getting Started:

* You will notice that I included a video for setting up a basic game with the pack. This video is still relevant and will work even with the updates to the pack. So if you wanted to get started with a free character model and environment pack, make sure you check out that video!
* Please note that the video uses UE 5.5 assets, and you will need to be on that version to use those packs together. If you want to use this with say a 5.4 metahuman, it will still work. However, the free Character Model and Environment were not built by me so I can't tell you if they work on an earlier engine version or not.
* I suggest replacing existing buildings by building your own, because the "Stairs" in the Environment pack are not properly angled for Unreal Engine default incline mechanics. If the building does not have any stairs then it really isn't an issue.
* After you get everything from the video set up, you need to place "Cover Points" and "AI Spawns" on the map for your AI.
* Below I included instructions for migration in the event that you would like to migrate my project or any parts of it into an existing project of your own.

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
