# Foul

Foul is our group project for Yoobee's BSE Second Year 205 Game Development Elective course: a Korean themed first-person shooter demo made in Unreal Engine 5.7.4. Our goal was to make a demo that sticks strictly to authentic Korean folklore and culture. You find a shotgun and try to survive against the pihaeja, an enemy that hunts you if it sees you, in a race to escape their hunt, you will come across some gate keys hidden away in their strongholds. Use those keys to escape and beat the demo.

This is the MVP version, so some things are still unfinished (see "Known issues" at the bottom).

## What's in the game

- A main menu with Start and Quit buttons
- First-person movement and camera
- A shotgun you pick up in the level and fire at enemies, with a muzzle flash, sound and random bullet cone spread
- Sound effects, like the shotgun firing and footsteps
- The pihaeja, an AI enemy that wanders around its own area and sometimes turns around randomly. If it sees you it chases you and attacks up close
- Player health, shown on a HUD with a crosshair and a health bar. The pihaeja can hurt you and if you die the level restarts and takes you to the main menu.

## What you need

- Windows 10 or 11 (64-bit)
- Unreal Engine 5.7.4, installed from the Epic Games Launcher. Other versions might not open the project properly
- Visual Studio with the "Game development with C++" workload. Unreal can need it for packaging, even if the project is mostly Blueprints
- About 100 GB of free space for the project, unreal engine and the build - demo build should only come to around 5GB space.

## How to install and build the game

We haven't included a ready-made exe. Instead you package your own playable version from the project, like this:

1. Download or clone the repo:
   ```
   git clone https://github.com/PrplManticore/Project-FOUL
   ```
2. Double-click `ProjectFOUL.uproject` to open it in Unreal Engine 5.7.4.
3. If it asks to rebuild, click Yes. The first load takes a while because of shader compiling.
4. Check the starting map is set. Go to Edit > Project Settings > Maps & Modes and make sure Game Default Map is `Lvl_MainMenu`.
5. In Project Settings > Packaging, make sure all our maps are in "List of Maps to Include in a Packaged Build" and set Build Configuration to Development.
6. Go to Platforms > Windows > Package Project.
7. Pick an empty folder to save the build in.
8. Wait for it to finish. The first time can take 10 to 30 minutes or more. You'll see "Packaging complete" in the bottom right when it's done. If it fails, open the Output Log to see why.
9. Open the folder you chose, then the Windows folder inside it, and run `ProjectFOUL.exe`. Keep the exe in that folder with the other files, because it won't run on its own.

If Windows warns you about an unknown app, click "More info" then "Run anyway".

If you just want to try it quickly without packaging, open the project in Unreal, open the map `Lvl_MainMenu` and press Play.

## How to play

Goal: [what the player is trying to do in the demo].

Controls:
- Move: WASD
- Look: mouse
- Jump: Space
- Shoot: left click (you have to pick up the shotgun first)
- Pickup Weapon: Walk into the gun you wish to equip and it will auto equip.
- Quit the game: Alt+F4 (or the Quit button in the main menu)

1. Press Start on the main menu.
2. Find the shotgun in the level and walk into it to pick it up.
3. Try not to stay in the pihaeja's line of sight. If it sees you it will chase the last place it saw you.
4. Shoot it before it gets to you. Keep an eye on the health bar. If your health runs out you die and the level restarts.

Tip: if you break line of sight it loses you and goes back to its home area.

## Known issues

- [e.g. pihaeja animations are still being worked on]
- [e.g. no ammo or reload - gun has unlimited ammo for now]

## Team

Will, Oskar and Eden.

All the assets in the game were made by us.
