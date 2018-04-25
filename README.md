Hello! If you're here, you're probably looking for some code samples of my work so here's a list of a few highlights.

If you'd like to browse all of my work, the full list of my repositories can be found [here.](https://github.com/droodicus?tab=repositories)



*******MOBA scripts

MOBA-style, top-down, right-click movement involves two C# scripts. The first is made for simply moving the controlled character to a selected empty space in the map (based on mouse position). The second is for pathing to a target enemy and starting an auot-attack loop on them when they are right-clicked.

[Basic movement script.](https://github.com/droodicus/MOBA_Champ_Simulation/blob/master/MOBA%20Champion%20Template/Assets/Scripts/Right_Click_Movement.cs)

["Chase and attack" script.](https://github.com/droodicus/MOBA_Champ_Simulation/blob/master/MOBA%20Champion%20Template/Assets/Scripts/Auto_Attack.cs)

The MOBA's turret targeting functionality is split between two C# scripts. One script is for detecting when enemy units enter or leave the turret's range and selecting a target based on this information. The other script is for shooting the bullet projectile based on a timer. It's worth noting that, like many traditional MOBAs, the turret's damage ramps up when repeatedly attacking the same target, but resets this scaling upon switch targets.

[Turret detection and target selection script.](https://github.com/droodicus/MOBA_Champ_Simulation/blob/master/MOBA%20Champion%20Template/Assets/Scripts/Turret_Detection.cs)

[Turret firing script.](https://github.com/droodicus/MOBA_Champ_Simulation/blob/master/MOBA%20Champion%20Template/Assets/Scripts/Turret_AI.cs)



*******FPS scripts

My FPS project is split between two selectable characters: One that uses a grappling hook and hitscan weapon, and another that uses a jetpack and projectile-based weapon (Overwatch players think Widowmaker and Pharah). First off is the jetpack system which uses a "fuel" resource (indicated on the UI by a gauge), with the addition of the ability to press Shift to use an additional upward burst of force.

[FPS dynamic jetpack system.](https://github.com/droodicus/FPS_Experimentation/blob/master/FPS/Assets/Scripts/Jetpack_Character/Jetpack.cs)

The grappling hook ability is split between two scripts. The first is attached to the character to shoot the grappling hook and pull themselves to it (once the grappling hook hits terrain). The second script is attached to the grappling hook itself, simply halting its movement and calling the casting character's Pull() function upon colliding with terrain.

[Player script to fire the grappling hook and pull themselves to it.](https://github.com/droodicus/FPS_Experimentation/blob/master/FPS/Assets/Scripts/Grapple_Character/Shoot_Grapple.cs)

[Grappling hook script to detect collision with the terrain.](https://github.com/droodicus/FPS_Experimentation/blob/master/FPS/Assets/Scripts/Grapple_Character/Grapple_Hook.cs)


*******WoW Talent Display

This project is less about writing program for games and instead accesses Blizzard's online databases using C# WebRequest system to retrieve a character's information, parse through it looking for specific keywords, and then outputting the relevant information (in this case, a character's talents based on their server and character name). 

[Full code can be found here.](https://github.com/droodicus/WoW_Talents_Legion/blob/master/Character_Info/Character_Info/Program.cs)
