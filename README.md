# gimp-photoshop
Making GIMP 2.10.38 work more like Adobe Photoshop


### Layer via Copy/Cut
Plugin to recreate Photoshop's `<control> j` functionality.

#### Installation:

1. Copy `plug-ins/layer-via-copy-cut.py` to your plug-ins folder.
   - For Flatpak, look here:
   `~/.var/app/org.gimp.GIMP/config/GIMP/2.10/plug-ins/`

2. Make it executable.

3. Start GIMP and look under the Layer menu for the last items.

4. [optional] add keyboard shortcut:
   - **Edit > Preferences**
   - Type in "layer via copy" and assign to `<control> j`
   - Type in "layer via cut" and assign to `<control> <shift> j`

5. Make sure "Save keyboard shortcuts on exit" is checked, then save and restart GIMP.


### Keyboard shortcuts

- http://epierce.freeshell.org/gimp/gimp_ps.php
- Here is a clone of the [menurc](menurc) file (in case the link above dies).


### Make "Snap to Canvas Edge" the Default

Something I find really frustrating in GIMP is that by default, layers don't snap to the edge of the canvas (or the grid) when I move them. Even worse, you have to enable it every single time you open an image.

- **Edit > Preferences > Image Windows > Snapping**
- Select "Snap to Grid" and "Snap to Canvas Edges" for both modes.
