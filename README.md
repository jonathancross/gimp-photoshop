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

### Disable "Show Layer Boundary" by Default

Something I never got used to in GIMP is the yellow and black dotted line that surrounds the active layer. Though it can be helpful at times, I definitely prefer to have it disabled by default.

1. From the main menu, navigate to **Edit > Preferences > Image Windows > Appearance**

2. Uncheck "Show Layer Boundary" for the modes you like.

3. Restart GIMP

You can always temporarily turn it back on by clicking on View in the main menu and choosing **Show Layer Boundary**.


### Make the Move Tool Function Like Photoshop's

By default, the Move Tool in GIMP is set to Pick a Layer or Guide. With this option set, it behaves a bit more like Inkscape or Illustrator because you can also move things that are not on the current layer (like the background). If you are a long time Photoshop user, this is very strange.

To make it function like Photoshop, you can set the default behavior to Move the Active Layer.

1. Select the **Move Tool** from the Tool Box in the left panel

2. In the **Tool Options** dialogue box check **Move the Active Layer**

3. From the main menu navigate to **Edit > Preferences > Tool Options > Save Tool Options Now**

4. Restart GIMP

----------------------------

Much of this guide was taken from these sources:

- https://www.linuxuprising.com/2018/11/configure-gimp-210-to-use-photoshop.html
- https://lifehacker.com/how-to-make-the-gimp-work-more-like-photoshop-1551318983
- https://github.com/cttynul/gimpshop-reloaded
- http://epierce.freeshell.org/gimp/gimp_ps.php
- http://gimpchat.com/viewtopic.php?f=9&t=4424


