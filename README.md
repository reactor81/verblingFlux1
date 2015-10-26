# Verbling Flux/React Challenge 1

## Version 1 - Essentials Only

### Background

This version has no extras added. See verblingFlux2 ad verblingFlux3 repos for Firebase Chat and WebRTC chat addons. 

### Features

#### Verbling Flummox

This implemention uses a Verbling fork of the Flummox Flux library (https://github.com/verbling/flummox). I actually created a fully working version of the Flux Challenge using my regular Flux framework (Alt) first. Once all functionality was complete, I decided to refactor to use Verbling's Flummox implementation to familiarize myself with this library. 

Comparing Alt and Flummox, I will definitely be using Flummox from now on. While they have many similar elements (e.g. registerAsync), I found Flummox to have less boilerplate. I like how actions automatically dispatch their return value, and I found the binding to actions in the store very easy. I also love the Store architecture - setState causing an emitChange is nicely modeled after React. Finally, <FluxComponent> connectToStores is great (I played with a custom render function to limit which state is passed down the tree in verblingFlux2 then decided it wasn't needed - but still excellent). 

#### Other Features

There should not be anything too surprising in this implementation.. API / WebSocket handling is done by 'Sources' in the /sources folder. I included a slightly modified Dispatcher to handle multiple action dispatches in same loop. This Dispatcher implementation is very short and light, but could certainly be improved upon. 

classnames package is included for easy manipulation of classNames styling. superagent is included as a light ajax library to avoid including all of jquery. ws is included to handle the websocket connection to server. 

### Install + Run

How to install and run

### Usage

As expected

### Author

Created by Daniel Guillamot - 2015-10-26