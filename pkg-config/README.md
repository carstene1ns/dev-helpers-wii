pkg-config
==========

This is a helper script that provides pkg-config support to build systems like
autotools or cmake for Wii homebrew compiling. It uses an exported variable
from devkitpro/devkitppc and points the hosts pkg-config to the right folder.


Installation
------------

After installing devkitpro/devkitppc you should have exported the environment
variable $DEVKITPPC and added the folder $DEVKITPPC/bin to your PATH. You can
then just copy the script 'powerpc-eabi-pkg-config' to this folder.

```
# cp powerpc-eabi-pkg-config "$DEVKITPPC/bin"
```
