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
| `na.applejuice.bar` | Montreal, Canada     |
| `eu.applejuice.bar` | Falkenstein, Germany |

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
/pregen <world> <radius> <type>
```

:::warning

`<radius>` is not `<diameter>`, if you want to host a `2000x2000` border game, you'd need to use `1000`.

:::

:::warning

Additionally, don't name your world `world`, `Spawn`, or `Arena`. Those worlds cannot be UHC worlds!

:::

:::info

Types: `cityworld`, `overworld`, `nether`

:::

For example, if I wanted to generate a `2000x2000` (diameter) world, you'd do `/pregen minota 1000 overworld`.

If you aren't happy with the way your world looks, you may cancel it! Use `/pregen cancel`, and then run the command again until you have something you want.

### Configuring your game

Some aspects aren't modified however, for example, the event times, game options, etc., so you need to configure that part yourself! 
Perform the command provided below to open the UHC Configuration:

```
/uhc
```

You should see a GUI pop up on your screen, this is the current UHC Configuration.
If you want to edit any value on the UHC Configuration, click any of the items, they should provide a GUI for editing any of the values.

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