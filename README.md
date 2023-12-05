# streamdeck-voicemeeter
*Work in progress.*

## Build Requirements
- Go 1.21.4 or later
- MSYS2

## Build and Run
You can build and run the plugin using the following command:

```bash
cd <project-root>
make run
```

This command will build the plugin, kill the running Stream Deck app, install the plugin, and run the Stream Deck app.

## Generate Layouts
Layouts describe how information is shown on the Stream Deck + touch display. Visit [Stream Deck SDK](https://docs.elgato.com/sdk/plugins/layouts-sd+) for more information.

First, create layouts using Draw.io and save it as a drawio file at `<project-root>/layout.drawio`.
Then, convert the layout to JSON files using the following command:
```bash
cd <project-root>
make layout
```

Output files will be generated in `<project-root>/layouts/`.
