# Uncommonsessions 1

Uncommonsessions is a neighbourhood for channeling a pluriverse design discourse. It engages with cross-educational models and operates at the intersection of design, open-source and politics. Hosting different channels rooted in a series of on/off line sessions, the collective infrastructure aims to connect alternative design practices facilitating the exchange of knowledge, resources and experiences. 



abc
## Source
Uncommonsessions uses https://github.com/cracker0dks/whiteboard as it main source while adjusting it to a more collaborative approach

## Some Features

- Shows remote user cursors while drawing
- Undo / Redo function for each user
- Drag+Drop / Copy+Paste Images or PDFs from PC and Browsers
- Resize, Move, Rotate & Draw Images to Canvas or Background
- Write text and sticky notes
- Save Whiteboard to Image and JSON
- Draw angle lines by pressing "Shift" while drawing (with line tool)
- Draw square by pressing "Shift" while drawing (with rectangle tool)
- Indicator that shows the smallest screen participating
- Keybindings for ALL the functions
- REST API
- Working on PC, Tablet & Mobile

## Install the App

You can run this app with and without docker

### Without Docker

1. install the latest NodeJs (version >= 12)
2. Clone the app
3. Run `npm ci` inside the folder
4. Run `npm run start:prod`
5. Surf to http://YOURIP:8080

### With Docker

1. `docker run -d -p 8080:8080 rofl256/whiteboard`
2. Surf to http://YOURIP:8080

## Designing

After you have installed the app, run `npm run start:dev` to start the backend and a frontend dev server. The website will be accessible on http://locahost:8080.

## URL Parameters

Call your site with GET parameters to change the WhiteboardID or the Username

`http://YOURIP:8080?whiteboardid=MYID&username=MYNAME`

- whiteboardid => All people with the same ID are drawing on the same board
- username => The name which will be shown to others while drawing
- title => Change the name of the Browser Tab
- randomid => if set to true, a random whiteboardId will be generated if not given aswell
- copyfromwid => set this to a whiteboardId you want a copy from. Only copies the content if the current whiteboard is empty.

## Configuration

Many settings of this project can be set using a simple `yaml` file, to change some behaviors or tweak performances.


**_ MIT License _**
