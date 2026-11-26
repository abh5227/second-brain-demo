# Second Brain, the demo

**Live demo: https://abh5227.github.io/second-brain-demo/**

Second Brain is my personal notes app. I send it a message or a photo, and it files each piece where it belongs, as plain Markdown files on my own laptop. It runs with no internet, and the model that sorts each message runs on the laptop too. I designed it and built it with Claude Code.

This repository holds only the built demo. The app's own code is in a private repository, because its history holds my personal notes.

## What is in this repository

- `index.html`, the page. It has the house, each room's text beside the app, the results, and what I learned.
- `app/`, a static build of the app's real screens. It holds the answers the demo shows (`app/demo-data.json`) and the made-up lecture files and record covers they point to.
- `vault.json`, the made-up vault's files and latest commits, which fill the drawing and the Basement.
- `fonts/`, IBM Plex Mono for the page's small labels. The app's own font, Archivo, is in `app/fonts/`.
- `THIRD-PARTY-NOTICES.md`, the libraries and fonts in the build, with their licenses.

There is no source code here to build from. One command in the private repository makes the demo, as described below.

## What is in the demo

- The app, drawn as a house at night. Each room is a section. Opening a room shows the real app on that section's screen, beside a few words about it.
- Three rooms show what is behind the walls. The Workshop is how a message gets sorted. The Basement is the vault, as its folders and its latest commits. The Attic is the night shift.
- The real screens behind every room: Today, the Inbox, the Calendar, Records, the Kitchen with its coffee map and grocery list, Shopping and gifts, Events, People and pets, Links, the Map, the Timeline, and Classes with a topic page and its review queue.
- A send box and six sample messages. In the app, a model on my laptop reads each message. Here, simple rules in your browser stand in for it, for the six samples and anything you type alike. They handle everyday phrasing, and anything they cannot read waits in the Inbox.

## What it is not

- Every name, note, record, café, receipt, and lecture in it is made up. The lecturers and slides in Classes are made up too, and the record covers are simple shapes drawn for the demo.
- Nothing you do leaves your browser. There is no server, no analytics, and no tracking. Edits last until you reload.
- The demo's day is fixed on the day it was exported, so its dates read as they did then.

## How it is made

One command in the private repository makes the demo. It writes a made-up vault, serves it with the app's real API, walks every screen in a browser, and keeps each answer. Then it builds the screens with a small stand-in that answers from those. Every name in the build is checked against my real notes before it is published.

The libraries and the fonts in the build are listed, with their licenses, in [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).
