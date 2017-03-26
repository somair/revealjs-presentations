# Reveal.js Presentations

This repository houses a simple base structure for creating, managing, and presenting multiple HTML-based presentations.  To create the presentations the excellent [Reveal.js](http://lab.hakim.se/reveal-js/) library is used.  For details on it please see the link provided.

## Fork This Repo

Firstly, it is intended that you fork this repository and then build presentations in your fork.  This repository just serves as the common structure and files needed to bootstrap things.  If desired you can occasionally pull from this upstream to get any updates to new library versions or whatever.  However, no guarantees can be made that your presentations will still work upon upgrade.

## Creating A New Presentation

Create a new folder inside the presentations folder that will house your presentation.  Copy the template.html file into your presentation folder and name it index.html.

Edit the index.html to contain your presentation slides, adjust styles to your liking, and otherwise customize your presentation.  For details refer to the Reveal.js documentation.

### Update the root index.html (optional)

If desired, you can update the root index.html to point to your presentation.  This makes things convenient when first pointing your browser at the served presentations.  It also serves as a nice index of all of the presentations you have created.  **NOTE:** This step will be automated with a script in the future.  At that time you will only need to run the script once every time you add a new presentation.

## Presenting

While presentations will mostly work by simply opening its index.html file in a browser a few features will be disabled in that scenario.

Instead, it is recommended to use the provided local web server, [Caddy](https://caddyserver.com/), to host your folder.  Simply execute the appropriate serve-* script for your given operating system.  Windows, Mac, and Linux are all supported.

Once you execute the given script, open a browser and point it to http://localhost:8080 and the root index.html should be displayed.  If you have updated it with your presentations you would simply need to click on the desired link and your presentation will begin.

### Speaker Notes

One of the advantages of using the provided web server is that speaker notes will work.  If you have written speaker notes, simply press S once you open your presentation and a second browser window will open to display the speaker notes.

## Special Thanks

I want to personally thank those individuals who have contributed to Reveal.js and to the Caddy Server projects.  The two, combined together here, make a very simple HTML-based presentation framework that is feature rich and yet still simple to use.
