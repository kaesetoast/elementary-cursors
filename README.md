elementary Cursor Theme
=======================

A cursor theme for elementary OS


###Installing 

Simple: copy the 'elementary' folder into '/usr/share/icons' and then set your cursor theme:

    gsettings set org.gnome.desktop.interface cursor-theme 'elementary'


###Using the Source

There are scripts to simplify the rendering process; to run them (and edit icons) you will need:

 * inkscape
 * python

To render the cursor theme from the [source plate](src/cursors/elementary.svg) you will need to run the render script in [src/cursors](src/cursors):

    python renderpngs.py

Then make the theme by running the make script in the [src/cursors/png](src/cursors/pngs) folder:

    bash make.sh

-----------