# m68K-AmigaOS-cross-compiler-setup-script
m68K-AmigaOS-cross-compiler-setup-script for Ubuntu 16.04 LTS (may be other debian based distrubition) to compile your Amiga OS 3.X C project
<br>
Compile your Amiga OS 3.X C project on Linux platform (Ubuntu) via AmigaOS cross compiler [https://github.com/cahirwpz/amigaos-cross-toolchain] <br><br>

Special Thanks to: <br>
@Alpyre [https://github.com/alpyre]<br>
@Simon [https://github.com/ozayturay] <br>
from www.commodore.gen.tr

# Usage
~~~~ bash
sudo sh ./m68k-amigaos-gcc-setup
~~~~

# Compile MUI Project
Do not forget add lines your source code to compile MUI project for Amiga OS 3.X with MUI3.8
~~~~ c
/* Otherwise auto open will try version 37, and muimaster.library has version
 * 19.x for MUI 3.8 */
int __oslibversion = 0;

/* We don't use command line arguments. */
int __nocommandline = 1;
~~~~
