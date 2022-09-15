---
sidebar_position: 2
---

# Hosting Guide

:::info


`<>` indicates required syntax, `[]` is optional syntax.


:::

## Before we begin
I (`minota#0887`) have gone out of my way to make hosting easy, if you have any suggestions however, please contact me on Discord!

## Posting your match
Dependent on the server you wish to host on, you must connect to the corresponding server. 

| **Server Address**  | **Location**         |
|---------------------|----------------------|
| `uhc.applejuice.bar` | Montreal, Canada     |

Then, you'd need to post a match to [hosts.uhc.gg](https://hosts.uhc.gg/). If you need assistance on posting on **uhc.gg**, please refer to the [Posting Guide](posting).

After you finished & you posted the game on **uhc.gg**, you need to get the matchpost ID, for example, my matchpost link would be `hosts.uhc.gg/m/6969`

What you'd need is the `6969` part, then with that matchpost ID, you perform the command:

```
/matchpost <id>
```

For example, you'd do `/matchpost 6969` with the example matchpost, doing this command will help the server identify your match & make the server automatically broadcast & open your game. This doesn't automate any processes like configuring the UHC Config & generating a world. 

### Generating a world

To generate a world, you must perform the command:

```
/pregen <name>
```

This will open up a pregeneration configuration GUI, which will allow you to configure your game better.

![Config](https://i.imgur.com/q6yiQtE.png)

This GUI is key to allowing you to create worlds.

#### Changing the border size

![Example](https://i.imgur.com/o0MKwsj.png)

The iron ingot is titled "Change Border", click it, this item allows you to configure your border size for your games.

![Example](https://i.imgur.com/K7Eqcav.png)

This will open up a GUI which will allow you to change the border size when you generate your world, left clicking will add **+50** to the number, and right-clicking will subtract **-50**, this border size is in radius as indicated by the **±** symbol, this means that the border in diameter would be **2000x2000** (if the number displayed is 1000x1000).

For example, I want to make my world **3000x3000** in diameter, I'd configure the border size in this menu to be **±1500**, as dispalyed here: 

![Example](https://i.imgur.com/Uj2R0zO.png)

#### Adding CityWorld to your game

Let's say you'd like to make your overworld a City World, that's simple! In the main pregeneration configuration GUI, click the redstone dust item. This will allow you to change the generation of the world. 

![Example](https://i.imgur.com/XAsZru3.png)

The *diamond block* allows you to change the generation type of your world, set this to **CITY_WORLD** to generate a City World game.

![Example](https://i.imgur.com/TY1UuQK.png)

#### Changing diamond/gold rates

Let's say you'd like to decrease the gold/diamond rate by **20%**, that -- my friend -- is also simple. In the main pregeneration configuration GUI, you should see the one unmentioned item, the paper item, click it. This will allow you to change certain settings for your game like *cane rates*, *diamond/gold rates* & remove *water/logs at 0,0*.

![Example](https://i.imgur.com/HL8n2Yc.gif)

#### Creating your world

After finally configuring your configuration to your pleasing, you'd click the emerald at the end of the main pregeneration configuration GUI, this will create your world based on the configuration given: 

![Example](https://i.imgur.com/CI2dob3.png)

This will begin to generate your world, visit your world using `/world tp <world name>`.

:::info

Don't like your world so far? Cancel it using `/pregen cancel` and try again!

:::


:::warning

Should the server be lagging from intensive generation, use `/pregen pause` to pause the current generation.

:::


#### OPTIONAL: Using generation commands

Let's say you have a scenario like `Underground Parallel` enabled, how would you generate the world using that scenario? It's simple actually! You must perform the command `/gen` after the pregeneration task has completed. This will then automatically generate your world based on the current scenarios that require generation.


#### OPTIONAL: Adding a nether world to your game

Let's say you want to link a nether world to your game, well, that's slightly simple! You must create a world named after your overworld world with the `_nether` suffix. For example, I typically call my worlds `minota`, so my nether world in this situation would be `minota_nether`. You must also change the world type in the generation settings to create said nether world.

### Configuring your game

Some aspects aren't modified however, for example, the event times, game options, etc., so you need to configure that part yourself! 
Perform the command provided below to open the UHC Configuration:

```
/uhc
```

You should see a GUI pop up on your screen, this is the current UHC Configuration.

![Example](https://i.imgur.com/WpowUVT.png)

If you want to edit any value on the UHC Configuration, click any of the items, they should provide a GUI for editing any of the values.

![Example](https://i.imgur.com/oAyE9z0.gif)

For example, if you wanted to turn *Absorption* off, you'd need to click the *Golden Apple* labeled **Game Options**, then you need to find the *Absorption* option & click it, then that option would be disabled, how simple is that?

:::warning

If you find any issues while trying to edit the configuration, please message me (`minota#0887`)! I'll try to fix it ASAP!

:::

## Editing teams

To edit the max size of teams, you'd perform the command:

```
/team size <number>
```

To lock/unlock teams, you'd perform the command:

```
/team management <on/off>
```

To reset teams, you'd perform the command:

```
/team reset
```

To set players to another team you'd perform the command:

```
/team set <player1> <player2>
```

In this case, `player1` would be set to `player2`'s team.


To create a team with multiple solos, you'd perform the command: 

```
/team ct <list of players>
```

Let's say a player named `minota` & `Grordbort` want to be teamed together, you'd perform `/team ct minota Grordbort`, this will create a team with the two solos together.

To see the rest of the team commands, you'd perform the command:

```
/team
```

## Starting a game

:::warning

**WARNING:** Before starting your game, you should be in Spectator Mode, this can be done by running `/spec`, this will prevent you from being scattered & help you run your game smoothly.

:::

To start a game, you'd perform the command:

```
/start <ffa/teams>
```

### Respawning players

In some situations, you must respawn the players, perhaps a hacker may have ruined your game and killed some players that you wish to respawn, now you can respawn them. Use:

```
/respawn <player>
```

**While they're in the server** to automatically add them back into the game with all their items back.

### Late-scattering players

Presume someone joins late, you'd likely want to late-scatter them, you'd need to perform the command `/ls` to late-scatter them, the usage is listed below: 

```
/ls <player> [optional teammate]
```

The optional teammate argument means that the first player gets teleported to that optional teammate & added to their team.

### Cancelling a game

Have a low fill? Unavailable to host your game? You're allowed to use `/cancel` in the server to cancel your matchpost, be sure to remove your matchpost on `hosts.uhc.gg` as well!

### Ending a game

Once a team/player ends up victorous, you must perform the command `/winner` on all winning players.

```
/winner <list of igns>
```

For example, me & Yobias just won a game, you'd set us as the winners using `/winner minota Yobias`.
Or, if you only wanted to set one winner as the winner, you'd do `/winner minota`.

This'll then count that player as a winner, then you are safe to do `/end` and finally end the game.

## Moderating your game

:::note

It's recommended to see the [Punishment Guidelines](punishments) on how (or how long) to punish a player.

:::

Moderation of your game is seriously recommended towards having a nice experience, banning hackers & resolving conflicts is recommended towards having a smooth game.

If you're hosting a game & you're in **Spectator Mode**, you'll see Mining Alerts & Combat Alerts of people mining & fighting, it's advised that you look at the activity as you could never know whether someone could be X-raying, Cheating, Flying, etc.

The commands you'd recognize from moderating your servers are made available to you, like `/ban`, `/mute`, `/kick`, `/warn`, `/banip`, etc. 

If you recognize a player as hacking, you must record evidence of them hacking (i.e. footage from a screenrecorder).

### Helpop

You're also given a feed of people asking for request, using `/helpop`, To reply to these requests, you may click on the message to be given a suggestion to help you reply to the help-op message.