Hello! If you're here, you're probably looking for some code samples of my work so here's a list of a few highlights.

If you'd like to browse all of my work, the full list of my repositories can be found at:
https://github.com/droodicus?tab=repositories



*******MOBA scripts

MOBA-style, top-down, right-click movement involves two C# scripts:

-The first is made for simply moving to a selected empty space in the map:
https://github.com/droodicus/MOBA_Champ_Simulation/blob/master/MOBA%20Champion%20Template/Assets/Scripts/Right_Click_Movement.cs

-The second is for pathing to a target enemy and starting an auto-attack loop on them when they are right-clicked:
https://github.com/droodicus/MOBA_Champ_Simulation/blob/master/MOBA%20Champion%20Template/Assets/Scripts/Auto_Attack.cs

MOBA's turret targeting functionality is split between two C# Scripts:

-One for detecting when enemy units enter or leave the turret's range and selecting a target based on this information:
https://github.com/droodicus/MOBA_Champ_Simulation/blob/master/MOBA%20Champion%20Template/Assets/Scripts/Turret_Detection.cs

-And one for actually shooting the projectiles based on a timer:
https://github.com/droodicus/MOBA_Champ_Simulation/blob/master/MOBA%20Champion%20Template/Assets/Scripts/Turret_AI.cs



*******FPS scripts

FPS dynamic jetpack system:
https://github.com/droodicus/FPS_Experimentation/blob/master/FPS/Assets/Scripts/Jetpack_Character/Jetpack.cs

Grappling hook ability is spit into two C# scripts:

-The first script is attached to a character to shoot the grappling hook and pull themselves to it (Once the grappling hook lands)
https://github.com/droodicus/FPS_Experimentation/blob/master/FPS/Assets/Scripts/Grapple_Character/Shoot_Grapple.cs

-The second script is attached to the grappling hook, simply halting its movement and calling the casting character's Pull() function upon colliding with terrain
https://github.com/droodicus/FPS_Experimentation/blob/master/FPS/Assets/Scripts/Grapple_Character/Grapple_Hook.cs



*******WoW Talent Display

This project is less about writing program for games and instead accesses Blizzard's online databases using C# WebRequest system to retrieve a character's information, parse through it looking for specific keywords, and then outputting the relevant information (in this case, a character's talents based on their server and character name):
https://github.com/droodicus/WoW_Talents_Legion/blob/master/Character_Info/Character_Info/Program.cs
