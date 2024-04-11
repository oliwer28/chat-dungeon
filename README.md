# chat-dungeon

The chat app made for dungeon dwellers. 

Dig into those deep conversations.

## Components

### The game - Frontend app

This is `Phaser3` application. It renders the game, accepts input from the player, displays where all other players are and their conversations.

### Server - cloud backend

#### AWS EC2 instance

This is our actual server - hardware itself. This is where our game is hosted and where it is syncing all players together.

#### Nginx

It is the reverse proxy, and it gives access to our game server.
This is where our `https` configuration lies. It is managed by the certbot from Lets Encrypt. 

#### Game server

This is the `Node.js` application which keeps all players interconnected and lets them see each other and talk.

## Development

Initial game generated from the official Typescript template. For all hints refer to their README file:
https://github.com/phaserjs/template-webpack-ts

### Requirements

[Node.js](https://nodejs.org) is required to install dependencies and run scripts via `npm`.
