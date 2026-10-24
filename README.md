# Next Stop — Transit Display Lab
An independent transit display simulation by Aliya Byrd.

## Open the project
Unzip the project and open index.html in your browser. The simulation needs no installation or build step.
To use the source viewer as well, serve the folder: `python -m http.server 8000`, then open http://localhost:8000.

## Files
- index.html: page structure, passenger display, and simulation controls.
- style.css: Arial typography, colors, route layout, and mobile styling.
- app.js: illustrative station data, rendering, journey timer, and button handlers.
- source.html: an in-browser code viewer.

## How it works
The stations array stores station names, transfers, and illustrative accessibility information.
index tracks the selected station. phase tracks traveling (0), arriving (1), or stopped (2).
Every 250 ms, the timer advances elapsed time at the selected speed. It changes phase and then station.
render() updates the text, badges, route map, progress bar, and control states.
switchView() switches between next-stop and route screens.

## Editing
Change stations in app.js to edit the journey. Change durations to adjust the three phases.
Edit style.css to change the display. All text uses Arial with system fallbacks.
The route is a 10-stop demo segment, not the complete A train route.
Station, transfer, and accessibility information is illustrative and not verified live data.
