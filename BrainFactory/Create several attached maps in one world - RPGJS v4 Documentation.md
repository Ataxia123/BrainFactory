[Skip to content](#VPContent)

[RPGJS v4 Documentation](/)

SearchK

Main Navigation[Home](https://rpgjs.dev)[Guide](/guide/get-started)[API](/commands/common)[Plugins](/plugins/chat)

Lean more

[Change Log](/others/changelog)

[Community](https://community.rpgjs.dev)

Appearance

Menu

On this page

Sidebar Navigation

API Preference

ModuleAutoload[?](/guide/api-preference "About API preference")

## Quick Start

[

Getting Started

](/guide/get-started)

[

Structure

](/guide/autoload)

[

Create your first map

](/guide/create-map)

[

Create hero in map

](/guide/create-sprite)

## Go further

[

Create World

](/guide/create-world-maps)

[

Add life bar, text or other above the player

](/guide/component)

[

Create event (NPC)

](/guide/create-event)

[

Create items

](/guide/create-database)

[

Create shape

](/guide/create-shape)

[

Add music in map

](/guide/create-sound)

[

Create animated tile

](/guide/animation-tile)

[

Save the player's progress

](/guide/save)

[

Production

](/guide/production)

## GUI

[

Customizing Your Theme

](/gui/theme)

[

Reusing GUI Components

](/gui/reuse-gui)

[

Creating Notifications in Your GUI

](/gui/notification-gui)

## Create GUI with VueJS

[

Creating Your Own GUI

](/guide/create-gui)

[

Adding Tooltips to Your GUI

](/gui/tooltip)

## Create GUI with React

[

Create Gui with React

](/gui/react)

[

Adding Tooltips to Your GUI

](/gui/react-tooltip)

[

Integrate in React App

](/gui/react-app)

## Technical

[

Environment Variables

](/guide/env)

[

All configuration in rpg.toml

](/guide/configuration)

[

Working with User Inputs

](/guide/inputs)

[

Supporting Gamepad Input

](/guide/gamepad)

[

Creating Responsive Game Design

](/guide/responsive-design)

[

Create Progressive Web Apps (PWA)

](/guide/pwa)

[

Add TailwindCSS

](/guide/tailwindcss)

[

Upgrade/Update RPGJS

](/guide/upgrade)

## Advanced

[

Create Authentication System

](/advanced/auth)

[

Synchronization between Server and Client

](/guide/synchronization)

[

Creating a plugin

](/advanced/create-plugin)

[

Using Agones for Game Server Hosting

](/advanced/agones)

[

Optimizing Performance

](/guide/performance)

[

Create Unit Tests

](/guide/unit-test)

## Web3

[

Authentification with wallet

](/web3/auth)

## Migration

[

v3 to v4

](/migration/to-v4)

On this page

Table of Contents for current page

- [Prerequisites](#prerequisites "Prerequisites")
- [Why ?](#why "Why ?")
- [Preview](#preview "Preview")
- [Preparing the world in the editor](#preparing-the-world-in-the-editor "Preparing the world in the editor")
- [Add the world to your game](#add-the-world-to-your-game "Add the world to your game")
- [Bonus. Prevent map change](#bonus-prevent-map-change "Bonus. Prevent map change")

On this page

# Create several attached maps in one world [​](#create-several-attached-maps-in-one-world)

## Prerequisites [​](#prerequisites)

- Have version 3.0.0-beta.8+
- Use Tiled Map Editor, and mainly the [World tool](https://doc.mapeditor.org/en/stable/manual/worlds)

## Why ? [​](#why)

The interest is to teleport the player on an adjacent map on consistent X and Y positions. You can also use a hook to tell if the player can change map or not

## Preview [​](#preview)

## Preparing the world in the editor [​](#preparing-the-world-in-the-editor)

Click on `World > New World` and add a file ending with the extension `.world` in

![create world](https://playground.rpgjs.dev/sandbox/224/assets/tiled-world.png)

Next, add maps to the world

![add in world](https://playground.rpgjs.dev/sandbox/224/assets/tiled-add-in-world.png)

1. Click on World Tool
2. Add the current map to a loaded

Place the maps so that the edges are touching

![tiled world](https://playground.rpgjs.dev/sandbox/224/assets/tiled-world-2.png)

## Add the world to your game [​](#add-the-world-to-your-game)

In `main/server/index.ts` :

ts

```
import { RpgServer, RpgModule } from '@rpgjs/server'
import myworld from './world/myworld.world'

@RpgModule<RpgServer>({
    worldMaps: [
        myworld
    ]
})
export default class RpgServerEngine { }
```

Just add JSON file in `main/worlds/myworld.world`

TIP

The world creates maps automatically and the map ID will be the file name. Be aware that if you already have a map with the same ID, the world will use this map

## Bonus. Prevent map change [​](#bonus-prevent-map-change)

There are several reasons for this. For example,

1. you can check that the character is on a dirt road (by looking at the tile ID)
2. You can make a scenario, if the player doesn't have the level, he can't change the map,
3. etc.

Go to and add `canChangeMap()` hook

main/server/player.tsmain/server/index.ts

ts

```
import { RpgPlayer, RpgPlayerHooks, RpgClassMap, RpgMap } from '@rpgjs/server'

export const player: RpgPlayerHooks = {
    // others hooks here...
    async canChangeMap(player: RpgPlayer, nextMap: RpgClassMap<RpgMap>): Promise<boolean> {
        if (nextMap.id == '<id of next map here>' && player.level < 10) {
            await player.showText('You can\'t go in that direction yet. You must have level 10 minimum!')
            return false
        }
        return true
    }
}

export default player
```

ts

```
import { RpgServer, RpgModule } from '@rpgjs/server'
import player from './player.ts'
import myworld from './maps/tmx/myworld.world'

@RpgModule<RpgServer>({
    player,
    worldMaps: [
        myworld
    ]
})
export default class RpgServerEngine { }
```

ts

```
import { RpgPlayer, type RpgPlayerHooks, type RpgClassMap, RpgMap } from '@rpgjs/server'

const player: RpgPlayerHooks = {
    // others hooks here...
    async canChangeMap(player: RpgPlayer, nextMap: RpgClassMap<RpgMap>): Promise<boolean> {
        if (nextMap.id == '<id of next map here>' && player.level < 10) {
            await player.showText('You can\'t go in that direction yet. You must have level 10 minimum!')
            return false
        }
        return true
    }
}

export default player
```

> Note that `nextMap` is not of type `RpgMap` because it is not loaded yet. It's only the class, so you can't get everything from it, e.g. the data of the next map

[Previous pageCreate hero in map](/guide/create-sprite)

[Next pageAdd life bar, text or other above the player](/guide/component)