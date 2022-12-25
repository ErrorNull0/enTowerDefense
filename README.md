# enTowerDefense

Battle an endless horde of zombies within an enclosed arena. Gameplay is focused on fast-paced action. There is no crafting or repairing, and building only consists of the basic cube blocks wood, cobble, concrete, and steel. Zombie kills give you coins, and all items are obtained from vending machines. If your health drops too low, you are knocked out, cannot move or attack, and a teammate must heal you, or you will bleed out and die. Once dead, you become a spectator and are free to roam the arena. But, you inflict no damage, while zombies mostly ignore you and cannot cause damage to you either. When all players die, the session is over, and a new game must be created to play again.


HOW TO SETUP:

- Copy the enTowerDefense mod into your Mods folder.

- Do not use any other mods with enTowerDefense. Mods that only tweak the on-screen HUD should be fine. Using any mods that modify items, zombies, player behavior, or anything else can cause unexpected behavior or errors.

- A custom map called "enTowerDefenseArena" is required. Copy this map into your "GeneratedWorlds" or "Worlds" folder. For single player, this is usually your "GeneratedWorlds" folder. On a dedicated server, the folder is typcially located in the Data > Worlds folder. Downloaded this map from github https://github.com/ErrorNull0/7D2D-Maps

- Use the default game time, 1 hour of real time = 24 hours of game time.

- Use the default Drop on Death option, set to "Everything"

- Use the default game difficulty, set to "Adventurer".

- Turn off player killing / pvp damage

- Turn off air drops. 

- Open gameevents.xml in a text editor and go to the section for "enAction_GiveCoins" (line 400). Find the property called "added_item_counts" and modify its value based on how many players will join the game. By default it is set to 40 which is intended only for single player. For multiplayer, divide $40 by the number of players and use that as the coin value above. Round that value to the nearest whole number. Example: 2 players = $20, 3 players = $13, 4 players = $10. 

Why do this? The 7 Days to Die engine automatically multiplies this coin reward for each number of players in the game. This behavior does not seem to have a way to disable. Setting this value lower for multiplayer counteracts this behavior and maintains a consistent coin reward. If this value is not modified lower for multiplayer, each player will gain more coins than designed, and disrupt the overall challenge.


HOW TO PLAY:

- The first player spawns into the enTowerDefenseArena map, and will appear next to a basic tower frame structure. The game time will be a few minutes before 7:00 AM. The game screen is in grayscale, because the game session has not begun.

- A weapons bag and loot crate will spawn close by that contains necessary items, which include a red pill, a stack of wood blocks, and a stack vending machines.

- Build a defensive area with your wood blocks on or around the tower frame, and place the vending machines in strategic areas for easy access. Note: the tower frame and vending machines are indestructable.

- For multiplayer, all players must be spawned into the map during this pre-battle period. Each player will receive their own weapons bag and loot crate.

- When ready for battle, eat the red pill and the screen will restore to full color. For multiplayer, the battle will begin only after all players have consumed their red pills. Once this happens, an alarm will sound indicating the start of the first wave of zombies!

- There are a total of 20 horde stages. Each stage lasts 3 hrs of game time, where 2.5 hrs of which zombies constantly spawn, and the final 30 min the spawning stops, and reward loot bags appear for player pick-up. Players can take this opportunity to repair or reinforce their defensive structure and use the vending machines.

- While progressing through each horde stage, tougher zombies will spawn. Upon reaching horde stage 20, zombie spawning will never end, no more reward loot bags will drop, and the goal is to survive for as many hours as possible beyond that point.

- Players start with 150 HP. If it drops below 50 HP, you get "knocked out", cannot move or inflict damage, and slowly bleed out. A teammate must heal you. Once your HP rises above 50, normal movement and attack ability is restored. If you die, you become a spectator and lose all of your items.

- As a spectator you cannot inflict damage nor receive damage, and zombies mostly ignore you. You are free to roam the arena with heightened movement speed and jumping ability. 

- When all players become spectators, game progression is no longer possible. Players can either give up and restart the game, or simply goof around the map as spectators for as long as desired.

- Note that for 25000 coins, a "resurrection shot" can be purchased from the vending machine which can revive spectators.



version 1.3
- zombies now spawn in waves (horde stages), with a total of 20 stages.
- created enclosed battle arena. stepping outside walls is instant death.
- added reward loot bag at the end of each horde stage.
- reward loot bags give progressively more loot as higher horde stages are reached.
- removed death penalty mechanic and removed stem cells from vending.
- added player "knock out" and "spectator" system
- disabled health and hunger mechanic nd removed food items from vending.
- added on-screen toolbelt meessages during certain events during gameplay.
- simplified weapon and armor selection in vending machines.
- increased bundle sizes of items to keep focus on action.
- added top tier machete "meat cleaver" 
- added top tier steel club "bone basher"
- removed snufkin zombies bosses and replaced with custom bosses.
- coin rewards scale better and much higher for tougher zombies.

version 1.2
- zombies no longer drop loot
- zombies now automatically provide coins up kills
- player spawns with vending machines for use to buy the needed equipment
- added a few Snufkin boss zombies for end game spawning

version 1.1
- added on-screen welcome at begining of session
- added 60s countdown at begining of session
- removed unnecessary weapons and ammo to reduce inventory clutter
- added weapon and armor mods and candy to loot
- added DanceBomb explosive that will cause all zombies to dance and be invincible for 60 seconds

