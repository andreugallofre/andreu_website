---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "TimeCube"
summary: |
  Cube that controls your time and you can manage it via web thanks to an API
authors: [ Marc Clascà, Víctor Sanchez, Carlota Catot, Andreu Gallofre ]
tags: [ arduino, react, dragonboard, node.js, express, mongodb, mongoose, google-cloud ]
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
url_code: "https://devpost.com/software/timecube"
url_pdf: ""
url_slides: ""
url_video: ""
links:
- name: GitHub
  url: https://github.com/andreugallofre/timecube
  icon_pack: fab
  icon: github

# Slides (optional).
slides: ""
---

# TimeCube
## Inspiration

We knew that every day, we waste a lot of time doing our tasks, and we usually don't have any way to control it, cause it's not easy to use.

## What it does

We've built a cube that controls your time and you can manage it via web thanks to an API. On the browser, you can associate tasks to every side of the cube, and when you turn the cube into that side, the server starts counting how much time you spend on that issue, task, ... (It's no only focused on the tech world, you can manage your time cooking, reading, etc.).

## How we built it

We run the frontend and the backend separately. The backend is built with node, express and mongo and it works as an API. the cube is built with a dragonboard and an arduino The Frontend has been developed with react.

## Challenges we ran into

Hardware is always difficult if you're not familiar with it. Deploying the API to the cloud and configuring servers. Comunicating with ourselves was a challenge to, cause everyone had their own idea on how to run it.

## Accomplishments that we're proud of

Deploying a functional API with just 24h,

## What we learned

Working better with branches in a git repo, working with different tech in the same proejct and learn to integrate them.

## What's next for TimeCube

The next step we would do with timecube is the integration with gitlab API that allows you to put the time you spend with every issue. Also, integrating with other general project management software so everyone can keep track of their tasks regardless of the area of their project.
