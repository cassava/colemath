# COLEMATH 1.0

This project is a modification (fork) of the excellent
[Colemak](http://www.colemak.com) keyboard layout.

It features the following modifications and additions:

  * Change of the CAPSLOCK key from Backspace to an additional ESC
    in the terminal version of the layout.

  * Inclusion of many useful math and greek symbols into the layout,
    in the form of an Xmodmap script (as it is intended for X11).

  * Inclusion of vim mappings, so that the hjkl navigation works.
    Only the keys that must be changed have been changed.

The Xmodmap scripts are put into /usr/share/colemath along with the
picture of the colemath keyboard layout. For these to be useful, they
need to be loaded with Xmodmap in your user session.
