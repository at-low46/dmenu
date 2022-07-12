at-low46's build of dmenu
============================

dmenu - dynamic menu
------------
[dmenu](https://tools.suckless.org/dmenu/) is an efficient dynamic menu for X.


Requirements
------------
In order to build dmenu you need the Xlib header files.


Patches
-------
The website has a [list of community patches](https://tools.suckless.org/dmenu/patches/).

The following patches were applied:

- [center](https://tools.suckless.org/dmenu/patches/center/)

To manually apply a patch, run:

	patch -p1 < path/to/patch.diff

To revert it, add the -R option:

	patch -p1 -R < path/to/patch.diff

Remember that patches only modify config.def.h, so you will need to manually replace/delete/update config.h before compiling.

Sometimes, after multiple patches, patching may fail and will require manual intervention. In that case, manually apply the unsuccessful modifications found in a newly generated file ending in a .rej extension.


Installation
------------
Edit config.mk to match your local setup (dmenu is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu
(if necessary as root):

	make clean install


Running dmenu
-------------
See the man page for details.

License
------------
In jurisdictions that recognize copyright laws, the following licenses apply:

[dmenu](https://git.suckless.org/dmenu/) is available under the [MIT/X Consortium License](LICENSES/MIT).

Everything made by me is under [The Unlicense](LICENSES/UNLICENSE).

For patches, refer to their individual pages linked above for details.
