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
As if it weren't obvious, you should probably be on the **applejuice** server. Connect using the IP below.

```
applejuice.bar
```

Then, you'd need to post a match to [hosts.uhc.gg](https://hosts.uhc.gg/). If you need assistance on posting on **uhc.gg**, please refer to the [Posting Guide](posting).

After you finished & you posted the game on **uhc.gg**, you need to get the matchpost ID, for example, my matchpost link would be `hosts.uhc.gg/m/6969`

What you'd need is the `6969` part, then with that matchpost ID, you perform the command:

```
/matchpost <id>
```

For example, you'd do `/matchpost 6969` with the example matchpost, doing this command will help the server identify your match & configure itself properly to help make some aspects of opening your game easier.

### Generating a world

To generate a world, you must perform the command:

```
/pregen <world> <radius> <type>
```

:::warning

`<radius>` is not `<diameter>`, if you want to host a `2000x2000` border game, you'd need to use `1000`.

:::

:::info

Types: `cityworld`, `overworld`, `nether`

:::

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

To start a game, you'd perform the command:

:::warning

Try to be in `/spec` mode before you perform the command, otherwise you'd be scattered & it'd be all messy.

:::

```
/start <ffa/teams>
```

If you want to latescatter players, use the command:

```
/ls <player> [optional teammate]
```

The optional teammate argument means that the first player gets teleported to that optional teammate & added to their team.

## Ending a game

Once a team/player ends up victorous, you must perform the command `/winner` on all winning players.

```
/winner <ign>
```

This'll then count that player as a winner, then you are safe to do `/end` and finally end the game.