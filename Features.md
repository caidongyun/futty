# List of features beyond the official PuTTY #
  * [PuTTYTray](http://puttytray.goeswhere.com/) and all the features it includes. (Thanks [Haanstra](http://haanstra.eu/putty/) and [FauxFaux](https://puttytray.goeswhere.com/))
    * Changes to PuTTYTray:
      * Updated [JK's file storage patch](http://jakub.kotrla.net/putty/) to v0.5 which supports jumplists. (Thanks [JK](http://jakub.kotrla.net/putty/))
        * See http://jakub.kotrla.net/putty/ for more info on using file based session/sshhostkey/jumplist storage.
      * Replaced the C++ Hyperlink detection with a C one. (Thanks [tobbez](http://ryara.net/putty-url/))
  * [PuTTYcyg](http://code.google.com/p/puttycyg/) ([Cygwin](http://www.cygwin.com) / Cygterm support) (Thanks [medgar123](http://code.google.com/p/puttycyg/))
    * Note: PuTTYCyg is made obsolete by [Cygtermd](http://www.chiark.greenend.org.uk/~sgtatham/putty/wishlist/cygwin-terminal-window.html).
  * [Adb support](https://github.com/yumeyao/PuTTY/commit/bef77b07135b98f5d238503c06001df6e51950b2) (Thanks [sztupy](https://github.com/sztupy/adbputty/commits/master) and [yumeyao](https://github.com/yumeyao/PuTTYTray)).
  * Added Window option called "Scrollback lines at a time". (Thanks [noodle1983](https://github.com/noodle1983/putty-nd))
    * Now you can scrollback a full screen or just a few lines at a time if you want.
  * Added the Terminal/Keyboard option called "Right-Alt acts as it is". (Thanks [ICE IV+putty](http://ice.hotmint.com/putty/))
  * Added Window/Behaviour option for "Switch FuTTY windows with Ctrl+Tab". (Thanks [ICE IV+putty](http://ice.hotmint.com/putty/))
  * [url-cut](http://koti.mbnet.fi/axh/putty-ntrans.html)
  * Option that allows maximizing but not resizing the window, where font sizes stay the same. (FireEgl)
    * It's the "Window" option called "Change rows and columns only when maximised".
  * Added mouse buttons option for "Middle pastes, Right brings up menu". (FireEgl)
    * The option is located under Window/Selection ..select "Default".
  * SSH related event logs show up on the terminal window as long as you're not logged in to the shell. (FireEgl)
    * To disable this, under Session/Logging, check "Omit session data".
  * IP ToS Support ([on XP/2003 only](http://support.microsoft.com/default.aspx?scid=kb;EN-US;q248611)). (FireEgl)
    * PuTTY & PuTTYTel = Low Delay
    * pscp & psftp = Max Throughput
    * plink = Max Reliability
  * Defaults to file based session storage unless you only have registry sessions, then it still loads the registry list by default. (FireEgl)
  * Ctrl+Tab for GNU Screen  (Thanks [johnLate](https://github.com/sewpafly/puttycygtray/commit/b760c9b6149d1248e930497c084486fb05934d0e))
    * To use this, put this in your ~/.screenrc file:
    * bindkey "^[[27;5;9~" next	# Ctrl-Tab
    * bindkey "^[[27;6;9~" prev	# Ctrl-Shift-Tab
    * Note, disable the Ctrl+Tab to switch PuTTY windows option to use this.
  * Added "Next Window	Ctrl+Tab" to the menu. (FireEgl)
  * Added support for combinations of Ctrl+/Shift+/Alt + Up/Down/Right/Left/Home/End to send the expected escape codes to the remote. (FireEgl)
    * Note, this changes what PuTTY sends for Ctrl+Arrows/Home/End, Home, and End.  I used mintty as a model, which seems to send the proper escape codes.
  * Made the config window taller and moved a few things around. (FireEgl)
  * Changed a lot of the default settings (fonts and colors mainly) (FireEgl).


---


It no longer contains these patches:
  * [transparency](http://sedlacek.biz/blog/putty/transparency/)
  * ["Reconnect" and "Save Current Session" menu options](http://dj1.willowmail.com/~jeske/Projects/Putty/)
  * [Remote-controlled (ANSI) printing to the Windows clipboard](http://ericmason.net/putty/putty-0.60-clip.patch)
But they can be added again if requested.