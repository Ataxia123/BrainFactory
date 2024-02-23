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
- [Step 1: Installation](#step-1-installation "Step 1: Installation")
- [Step 2: Set Up a Basic GUI](#step-2-set-up-a-basic-gui "Step 2: Set Up a Basic GUI")
- [Step 3: Incorporate Context](#step-3-incorporate-context "Step 3: Incorporate Context")
- [Step 4: Interact with the Server Side](#step-4-interact-with-the-server-side "Step 4: Interact with the Server Side")

On this page

# Building GUI with React [​](#building-gui-with-react)

## Prerequisites [​](#prerequisites)

- You must be familiar with the [React](https://react.dev) library
- Since v4.1.0

WARNING

**Experimental Feature**: This feature is still in its experimental stage and may not be stable.

## Step 1: Installation [​](#step-1-installation)

Begin by installing the necessary dependencies:

bash

```
npm install react react-dom
```

## Step 2: Set Up a Basic GUI [​](#step-2-set-up-a-basic-gui)

In the file `main/gui/mygui.tsx`, create a simple React component:

tsx

```
export default function MyGUI() {
  return (
    <div>
      <h1>Hello World</h1>
    </div>
  );
}
```

Name function is used for identifying the GUI. Id is `my-gui`.

> Id is Kebab Case of the name function

## Step 3: Incorporate Context [​](#step-3-incorporate-context)

For more dynamic data, you can utilize the context from the RPG client and some React hooks.

tsx

```
import { RpgReactContext } from '@rpgjs/client/react';
import { useContext, useEffect, useState } from 'react';

export default function MyGUI({ foo }) {
  const { rpgCurrentPlayer } = useContext(RpgReactContext);
  const [hp, setHp] = useState(0);

  console.log(foo);

  useEffect(() => {
    const subscription = rpgCurrentPlayer.subscribe(({ object }) => {
      setHp(object.hp);
    });
    
    return () => {
      subscription.unsubscribe();
    };
  }, []);

  return (
    <div>
      <h1>{hp}</h1>
    </div>
  );
}
```

## Step 4: Interact with the Server Side [​](#step-4-interact-with-the-server-side)

On the server side, you have the capability to open the GUI for players.

In the file `main/player.ts`:

ts

```
import { RpgPlayer, RpgPlayerHooks } from '@rpgjs/server';

const player: RpgPlayerHooks = {
  onJoinMap(player: RpgPlayer) {
    player.gui('my-gui').open({
      foo: 'bar' // You can send props to the GUI
    }); 
  }
};

export default player;
```

[Previous pageAdding Tooltips to Your GUI](/gui/tooltip.html)

[Next pageAdding Tooltips to Your GUI](/gui/react-tooltip.html)