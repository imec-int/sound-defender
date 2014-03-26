# Sound Defender

Defender-like game, where enemies are rendered based on MIDI data, landscape based on audio,
and where the planes are controlled remotely with a smartphone or tablet.

## Changes by MiX
* we've moved everything to ```app/public/``` and moved the content from ```sound-defender-backend/``` to the ```app/``` folder so everything accesible from the same project.
* we've updated the file references accordingly.
* we've change every absolute reference of socket.io to a relative reference so that there are no hardcode ip adresses in the code.
* we've chnaged ```app.listen()``` so that we can run the server on a port other than port 3000.
* added a ```.gitignore```
* updated readme so that it matches the other hacks from the hacktathon

## Installation

### Install Node.js
* Get Node.js from http://nodejs.org
* Install it

### Install Dependencies
Run
    
    npm install

from the ```app/``` folder.

## Running the code

run

    node app.js

from the ```app/``` folder.

Or run

    PORT=4000 node app.js

To run it on another port (eg port 4000)


### Visuals

Plug in the audio cable on your desktop pc, open your desktop browser and go to

    http://localhost:3000/host.html

### Smartphone interface

With your smartphone, go to 

    http://localhost:3000/

and if a plane is assigned to you, start playing!

## MIDI input

This project uses the MIDI data that was available at the hackthon.

In ```public/host.html``, change the location of the MIDI api if nessesary:

     <script src="http://mixmini.mixlab.be:3000/javascripts/api.js" type='text/javascript'></script>


If you want to run the MIDI api yourself, you can clone the ```https://github.com/mixbe/mixmidi``` project.
