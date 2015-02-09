elementary Cursor Theme
=======================

A cursor theme for elementary OS


###Installing 

Simple: copy the 'elementary' folder into '/usr/share/icons' and then set your cursor theme using your favourite tool or:

    gsettings set org.gnome.desktop.interface cursor-theme 'elementary'

But to make a system-wide change run the following:

    sudo update-alternatives --install /usr/share/icons/default/index.theme x-cursor-theme /usr/share/icons/elementary/cursor.theme 91

Then use the following to choose 'elementary':

    sudo update-alternatives --config x-cursor-theme


###Using the Source

There are scripts to simplify the rendering process; to run them (and edit icons) you will need:

 * inkscape
 * python

To render the cursor theme from the [source plate](src/cursors/elementary.svg) you will need to run the render script in [src/cursors](src/cursors):

    python renderpngs.py

Then make the theme by running the make script in the [src/cursors/png](src/cursors/pngs) folder:

    bash make.sh

-----------