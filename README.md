# AppKit

Our AppKit: the classes of AppKit of the Mac written back from the decompile (`decompiled/src`, one `NS*.m` per class, with tests in `decompiled/test`) and the backend that puts them on the window server (`decompiled/src/Open*.m`: windows, events, text, nib loader, documents, menus, panels, colours, theme).

It is built on a Mac as `/open/AppKit` (see `pearOS-bsd/open`: `build-appkit.sh`) and unmodified Mac applications run on it.  It needs `WindowServer` (client library, `WINDOWSERVER_DIR`), `SkyLight` (`SKYLIGHT_DIR`) and `CoreUI` (colours and window buttons from `.car` files).
