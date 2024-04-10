# chat-dungeon

The chat app made for dungeon dwellers. 

Dig into those deep conversations.

## Components

### The game - Frontend app

This is Phaser3 application. It renders the game, accepts input from the player, displays where all other players are and their conversations.

### Server - cloud backend

#### AWS EC2 instance

This is our actual server - hardware itself. This is where our game is hosted and where it is syncing all players together.

#### nginx

It is the reverse proxy, and it gives access to our game server.
This is where our https configuration lies. It is managed by the certbot from Lets Encrypt. 

#### game server

This is the nodeJS application which keeps all players interconnected and lets them see each other and talk

## Development

Initial game generated from the official Typescript template:  
https://github.com/phaserjs/template-webpack-ts

