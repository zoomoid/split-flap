# split-flap

This repository tracks development of a design experiment of implementing a historic artifact of larger train stations and airports: The Split-Flap Display.

Those electromechanical display boards operate with a roll for each character or digit in a matrix, most commonly for arrival and departure times, that rotate through their character set until reaching their desired glyph. The characters are cut horizontally to compress the number of flaps for each roll by using front and back of each flap for different flaps for a singular character.

![split-flap display animation](https://upload.wikimedia.org/wikipedia/commons/8/84/Split-flap_display_2016-01-17.gif)

Their aesthetic effect and their mechanical sound has been used by various artists in the past and a digital recreation of this mechanism has been on my bucket list for a long time.

## Development

This project uses HTML5's canvas element to draw the characters. To make handling the javascript API a little less tedious, we rely on [paper.js](https://github.com/paperjs/paper.js) for the drawing context.

Furthermore, to ease development, we opted for Vue 3 + vite.js to drive the project's frontend.