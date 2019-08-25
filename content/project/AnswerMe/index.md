---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Answer Me, Will you?"
summary: |
  We go out so often together and we don't have many fun games to enjoy while drinking, so this is it! 
authors: [ Guillem Ramírez, Andrea Querol, Víctor Sanchez, Andreu Gallofre ]
tags: [ code, website, noode.js ]
categories: [ source ]
date: 2018-11-11T11:23:56+02:00

# Optional external URL for project (replaces project detail page).
external_link: ""

# Featured image
image:
 caption: ""
 focal_point: ""
 preview_only: false

# Links
url_code: "https://devpost.com/software/answer-me-will-you"
url_pdf: ""
url_slides: ""
url_video: ""
links:
- name: GitHub
  url: https://github.com/teleportex/web_app_socket
  icon_pack: fab
  icon: github

# Slides (optional).
slides: ""
---

# Answer Me Will You

## Inspiration

We go out so often together and we don't have many fun games to enjoy while drinking (water or soda) and we wanted to create a fun app that people form all the world :P

## What it does

It's a Truth or Dare like game that allows you to play with your friends with a default set of questions/challenges or create a new one for more fun. We build a lobby with rooms, so you can play with your friends and multiple instances of the game can run at the same time, begin updated simultaneous to all clients.

## How we built it 

We build it with node.js, sql and sockets.io for the backend and javascript, html5 and css3 for the frontend. And for the databases we used an IBM instance to have the database synchronized at all times.

## Challenges we ran into

Socket.io communication was a pain in the ass for sure, we had many problems when we had to update all clients connected to a room. Also, some of the database communication was kind of messy because we only have 5 connections at the same time.

## Accomplishments that we're proud of

Well, everything, it was our first hackathon together working with technologies that we were using for first time and was so nice to see what we were able to accomplish.

## What we learned

As we said before, it's our first time with that kind of technologies so in 24h we have learned fronted, backend, socket communication, databases, cloud deployment.... =)

## What's next for Answer me, will you?

We will add new games in a near future, maybe making an app from the website and improve some internal systems
