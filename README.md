# 3D_Visualization_API
My project goal for this project is to create a software library that can be integrated in Liquid Galaxy, that allows third parties to easily apply common features in Computer Graphics directly to a Liquid Galaxy format, a multi screen display cluster launching instances of Chromium OS in each machine. This would include really commonly used properties in graphics, modelling a geometric object, applying lightning, animation, shaders and even textures.

## Getting Started

### Prerequisites

This project is created using Socket.io and you need to have Node and npm (node package manager) installed. If you do not have these, head over to Node setup to install node on your local system. Confirm that node and npm are installed by running the following commands in your terminal.
```
node --version
npm --version
```
And you should get something similar to
```
v5.0.0
3.5.2
```

### Installing

In order to run the project, the steps are:

```
npm install
nodemon app.js
```
If there is problems running the last command try typing npm install -g nodemon

And then you can open a browser and go to http://localhost:3000/

The order for opening the browsers to have a decent view  would be:

![Alt text](orderConnecting.png?raw=true "Order for connection of browsers")


#### Installing in different machines

You need all machines to be connected to the same network. You will still need to install the dependencies:
```
npm install
```

However you only need to run one server, so for the central screen run :
```
nodemon app.js
```
And in that machine, you can open a browser and go to http://localhost:3000/. For the rest of screens, just open the browser and go to the same link but with the IP Address instead of localhost, which can be found on top of the browser (might need to scroll a little bit).

The order of connection would still be the same.

## Controls
* w → moves forwards (translate camera negatively on the Z axis)
* s → moves backwards (translate camera positively on the Z axis)
* a → moves left (translate camera negatively on the X axis)
* d → moves right (translate camera positively on the X axis)
* space bar → moves up (translate camera positively on the Y axis)
* x →  moves down (translate camera negatively on the Y axis)
* left/right key → rotates around Y axis
* up/down key → rotates around X axis
* q/e → rotates arounds Z axis

## Built With

* [Socket.io](https://socket.io/) - Library for web sockets
* [Threejs](https://threejs.org/) - Graphics library
