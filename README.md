Sound Defender
=======

Defender-like game, where enemies are rendered based on MIDI data, landscape based on audio,
and where the planes are controlled remotely with a smartphone or tablet.

Installation
=======

1. Install the backend server from https://github.com/myster0n/sound-defender-backend
  npm install
  nodejs index.js

2. Check out these static files and put them on a web server

3. open host.html and index.html in a text editor, and change the location of socket.io:

  <pre>
  ...
  <script src="http://lacerta.be/socket.io/socket.io.js"></script>
  ...
  var socket = io.connect('http://lacerta.be');
  </pre>

4. In host.html, change the location of the MIDI api:

  <pre>
  <script src="http://mixmini.mixlab.be:3000/javascripts/api.js" type='text/javascript'></script>
  <pre>

4. Plug in the audio cable on your desktop pc, open your desktop browser and go to http://your_web_server/sound-defender/host.html

5. With your smartphone, go to http://your_web_server/sound-defender/ and if a plane is assigned to you, start playing! 
