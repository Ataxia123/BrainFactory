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

- [What is RPGJS?](#what-is-rpgjs "What is RPGJS?")
- [Technology](#technology "Technology")
- [Compatibility](#compatibility "Compatibility")
- [Installation](#installation "Installation")

On this page

# Get Started [​](#get-started)

## What is RPGJS? [​](#what-is-rpgjs)

RPGJS was created several years ago, with the aim of creating an RPG on the browser. For this, the framework uses HTML5 Canvas. However, it was not possible to make only RPG. Currently, the version of RPGJS allows you to create an RPG or an MMORPG at the same time.

## Technology [​](#technology)

- Typescript v5
- ViteJS v4 (for compilation)
- NodeJS v18+ (for server)
- Socket.io v4 (for real time)
- PixiJS v7 (for WebGL rendering)
- VueJS v3 (for GUIs)

## Compatibility [​](#compatibility)

**Client-Side**

- Google Chrome
- Firefox
- Edge (only Webkit version)
- Brave

> Warning, the game is not compatible with Internet Explorer.

**Server-Side**

- NodeJS 18+

## Installation [​](#installation)

**For MMORPG**:

bash

```
npx degit rpgjs/starter my-rpg-game
cd my-rpg-game
npm install
npm run dev
```

And open a browser on `http://localhost:3000`

> To change the port: `PORT=4000 npm run dev`. Then, you can go to port 4000

**For RPG**:

The same line as above but start the development line with `RPG_TYPE` environment variable:

`RPG_TYPE=rpg npm run dev`

Go to `http://localhost:3000`

> To change the port: `PORT=4000 RPG_TYPE=rpg npm run dev`

For Windows

To use the environment variables, it is different from Linux

So use the package cross-env

```
npm install --save-dev cross-env
npx cross-env RPG_TYPE=rpg npm run dev
```

[Next pageStructure](/guide/autoload.html)