---
layout: post
title:  "Prototype: Phase 2"
date:   2019-04-11 4:38:53 -0600
categories: [ Capstone ]
---

# Collaborative Canvas

This prototype focuses on the implementation of collaborative web interfaces.

[**Demo App**](https://draw-collab.herokuapp.com/)


<img src="{{ site.baseurl }}/assets/image/capstone-1/collab-canvas.png" alt="screenshot" style="width:550px;"/>

Each user is assigned a different color when visiting the website. Clicking a cell in the grid colors the cell or removes the color. Other user's pointer positions are displayed as colored dots. Collaboration is encouraged by assigning each user a single color. This has the effect of dividing tasks among users.

## Demo Video

<iframe src="https://player.vimeo.com/video/330075481" width="550" height="413" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>

## How did I do this

The main technologies used in this project are [React.JS](https://reactjs.org/) and [Socket.io](https://socket.io/). Socket.io is a JavaScript library for realtime web apps. The main advantage of this library is that it enables persistent two way communication between client and server applications. This is accomplished by using the standard WebSocket protocol with long-polling as a fallback.

The state of the canvas is stored and maintained on the server. When a client connects, the server sends it the current state of the canvas to be rendered. When a user interacts with the UI a message is sent to the server with the pixel position and the new color. This message is then broadcasted to all connected clients. 

[**Github**](https://github.com/LucasDachman/draw-collab)

## Reflection 

This is a quick and dirty prototype. Here are some problems:

#### No limit on how many users can edit the canvas at once

This not really a problem—It's an obstacle. Having more than 10 people connected introduces lag. This can be overcome in a few ways. (1) Limit the amount of users. (2) Optimize the server code. (3) Scale the server. If the server can't handle the volume of requests, I can scale it by creating more servers with the same code and load-balancing between them. This would be difficult if the servers need to share state. 

Limiting the number of users may have other advantages besides reducing the load on the server. Collaborating with too many people can introduce chaos. There may be a limited number of tasks to assign. Should users be able to share tasks?  

#### Tasks (colors) are assigned randomly

Assigning single colors to individual users has the effect of separating tasks between users. This is great but I'd like users to have more options. Maybe users can swap roles or select from a pool of roles. If there are only two users but five available tasks, users should be able to change roles. 

#### Sessions are not persistent

If a user refreshes the page the server sees this as a client closing a connection and a new client creating a new connection. In the case of this app, the effect is that the user is assigned a new color. To fix this I can make better use of session keys with IP addresses. It would also be nice for users to have the ability to create usernames that are displayed in the app. 

#### Not mobile friendly

This is just a matter of layouts and media queries (gross)

## Takeaways & Future Directions

The collaborative interface turned out to be pretty easy to implement. The hard part will be integrating audio and synthesis. Audio lag or glitching is much more jarring to a user than GUI lag. I'll need to be strategic about how tasks are separated between server and client. It may be possible to only send control signals from the client and render all audio on the server then broadcast that audio to all clients. If there is too much lag, I may have to only send control signals between server/client and render the audio in the browser.  

