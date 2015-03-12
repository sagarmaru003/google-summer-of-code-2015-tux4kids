# Note: #

  * To discuss your possible proposals, you can subscribe to the tux4kids-discuss mailing list and post it there. http://lists.alioth.debian.org/cgi-bin/mailman/listinfo/tux4kids-discuss

  * These are sample ideas, not necessarily pre-canned projects that can be selected without further research. Please study the relevant source code and put together a well-written proposal of what you would like to accomplish over the summer.

# Tux English #
**Tux4Eng is a very new and fresh idea need to be start from scratch and designed for kids to learn basic English in which kids can start from typing letters and can reach to solve word maze and sudoku. This game is the most basic game and currently We have developed beta version of it. By playing this game kids can learn alphabets by visualising the shapes of it and then by clicking the squares.**

**_Implementation and Library:_**This game is implemented using HTML, CSS, Javascript and Phaser library. The reason of using this library is that this game can be deployed on different platforms according to the requirement. While designing the game we also took mobile and tablets versions into consideration. This game has a user interface which is compatible with both touch screen phone and laptops.

**_Explanation:_** http://goo.gl/Lczy3U
**_Mentor:_** aaditya025@gmail.com


# Tux Mind Exercise #

**Tux4ME** is a very new and fresh idea need to be start from scratch and designed to develop and enhance mental power. It include a series of game, each testing and improving player’s

**reasoning capabilities** speed
**attention** flexibility
**memory power**

There will be simple games, which would take couple of minutes so that you can play them daily. This will help you to exercise your brain to make it active and healthy. It is kind of mental ability development software where people can test and improve their reasoning capabilities, speed, attention, flexibility and memory power. It is a combination of fun and self improvement.

**_Implementation and Library:_**This game is implemented using HTML, CSS, Javascript and Phaser library. The reason of using this library is that this game can be deployed on different platforms according to the requirement. While designing the game we also took mobile and tablets versions into consideration. This game has a user interface which is compatible with both touch screen phone and laptops.

**_Explanation:_** http://goo.gl/D5PR17
**_Mentor:_** aaditya025@gmail.com


# Tux Paint #
  * Website: http://www.tuxpaint.org
  * CVS repositories - See http://sourceforge.net/scm/?type=cvs&group_id=66938
  * [Browsable link](http://tuxpaint.cvs.sourceforge.net/tuxpaint/)

  * **_Wallpaper tool/mode like the pattern magic tool that affects the behavior of the overall program:_** The goal is to provide a paint mode that is able to create tileable draws that match side by side forming a mosaic. There is a magic tool aimed to small children that does this, it has several limitations like fixed size of the pattern and fixed size of the brush. You should do the same behavior for the overall program, so one can choose the size of the pattern, the brushes, stamps or text to apply.
    * Prerequisites:
      * C necessary
    * Difficulty: easy


  * **_Port  to Android, IOs...:_** Currently tuxpaint is being ported to the SDL2 library, that means that it will be able to run on the newer platforms supported by SDL2.
  * Git repository: https://sourceforge.net/p/tuxpaint-sdl2/code/ci/master/tree/
    * Prerequisites:
      * C necessary
      * Java
      * Android/IOs knowledge
    * Difficulty: Hard
**_Mentor:_** perepujal@gmail.com

# Tux Math #
  * Website: http://tux4kids.alioth.debian.org
  * Git repositories for read-only cloning:
    * git://git.debian.org/git/tux4kids/tuxmath.git (tuxmath proper)
    * git://git.debian.org/git/tux4kids/t4kcommon.git (t4k\_common library)
    * Browsable links also available at: http://tux4kids.alioth.debian.org/git.php

  * **_Migrate Tux Math and t4k\_common to SDL 2.0:_**  SDL 2.0 was recently released, and offers many potential advantages for future development. For example, applications are no longer limited to a single window.  For this project, a minimum objective would be to adapt all of the function calls and platform builds to use SDL 2.0.  It should be noted that we have historically provided support for builds with both GNU Autotools and CMake.  We also provide cross-platform builds for Windows using  [mingw-cross-env](http://mingw-cross-env.nongnu.org/), and for OS-X with [MacPorts](http://www.macports.org).
    * Prerequisites:
      * solid knowledge of C/C++ required.
      * some familiarity with build systems and SDL highly useful.
      * will need to know or learn how to use Git.

  * **_Create unit tests for Tux Math and t4k\_common:_** Tux Math currently lacks any built-in mechanism to test for run-time errors as part of the build process.  Both Tux Math itself and t4k\_common could benefit from integrated testing capabilities.  For example, for Tux Math, the basic idea would be to create a runtime "--test" flag that would cause the program to systematically load all date, execute all important code paths, log relevant data, and exit with meaningful values according to the success or failure of the component tests.
    * Prerequisites:
      * solid knowledge of C/C++ required.
      * familiarity with concept of Testing Driven Development

_**Mentor:**_ deepak.aggarwal9@gmail.com

# Tux Typing #
  * Website: http://tux4kids.alioth.debian.org
  * Git repositories for read-only cloning:
    * git://git.debian.org/git/tux4kids/tuxtype.git (tuxtype proper)
    * git://git.debian.org/git/tux4kids/t4kcommon.git (t4k\_common library)
    * Browsable links also available at: http://tux4kids.alioth.debian.org/git.php

  * **_Adapt Tux Typing to use the t4k\_common library:_** Tux Typing and Tux Math have long shared a significant amount of code in an informal, copy/paste manner.  The t4k\_common library was created to handle this in a better fashion, and recent releases of Tux Math have used t4k\_common.  However, Tux Typing has not yet undergone this transition.  It also has a significant amount of very old code that needs maintenance.  This project will nearly be a rewrite of the Tux Typing code base, apart from the game activity source files themselves.
    * Prerequisites:
      * Good C/C++ skills most important
      * Git, Autotools, CMake, SDL all very helpful.

  * **_Create a LAN multiplayer mode for Tux Typing:_** Tux Math has a LAN mode, where kids can compete against each other to answer the same questions the quickest.  For this project, you could adapt the existing "Fish Cascade" game for cooperative network play, or come up with an entirely new game design (e.g. - have Tux swim toward a goal, with his progress proportional to the player's typing speed).
    * Prerequisites:
      * C/C++ necessary
      * Some knowledge of C network programming (SDL\_net or straight BSD sockets) very useful.
      * As with other projects, familiarity with Git/Autotools/CMake will be needed or learned during project.

  * **_Improve Input Method (IM) support for Asian (and potentially other) languages:_** Tux Typing is well-internationalized for display. It is capable of displaying any Unicode character for which the system has appropriate font.  However, it has significant limitations regarding proper handling of keyboard input of non-ASCII characters.
> > The most critical limitation is that the program cannot handle languages that require multiple keypress events to type a single character (e.g. Chinese, Japanese, Korean).  Tux Paint does handle such input correctly.  The IM code from Tux Paint has been copied into Tux Typing and partially adapted, but it is not yet used by the program.
> > A second issue is that the accents and other non-US characters used by other Western languages (French, Spanish, German, many others) are generally not "typable".  This appears to be simply a bug.  While bug fixing is not in itself an acceptable GSoC project, it would be highly appropriate to address this issue as part of improving the robustness of Tux Typing's internationalization.
      * Prerequisites:
        * C/C++ necessary
        * Good knowledge of i18n, Unicode, character encodings, and GNU Gettext.
        * Knowledge of git/cvs and build systems highly advisable.

# Tux4kids Mobile #

  * **_Transition the Tuxmath mobile app from a prototype to release stage_** A port/re-implementation effort during the previous Google Summer of Code was undertaken to target mobile platforms. The port is in an alpha stage currently - https://github.com/tux4kids/tuxmathmobile. Responsive UI design, logging framework, i18n, improvements and addition of game mechanics are some of the challenges you will be facing in this project. This project requires a high degree of software engineering rigor as you will be frequently releasing the app to the Play/App store.
  * Project difficulty: _Medium to high_
  * Prerequisites:
    * _HaXe NME:_ NME is a HaXe (a multi-platform programming language) based  open-source framework, which provides cross-platform support for Android, iOS, HTML, and Flash among others out of the box. The development is supported on Windows, Linux and Mac platforms. HaXe will look very familiar if you are coming from an AS3 background. Both can be picked up on the fly while working on bugs.
    * _Git:_ An intermediate knowledge of Git is a must.
  * Contribution guide:
    * Fork https://github.com/tux4kids/tuxmathmobile, fix bugs, and send pull requests.
    * Add documentation support in the wiki.
    * Add bugs/issues in the issue tracker.

  * **_Develop Mobile applications for Tux4kids_** This "Idea" has a great deal of flexibility. The main goal is to extend our project beyond installed desktop software into such areas as web-based applets and educational games for mobile platforms (Android and iOS).
> > Although there is some possiblity of working with the current code bases via the SDL ports for these platforms, it is probably more advantageous to write these as new apps from scratch.  In particular, the GPL3+ license of Tux Math and Tux Typing is not compatible with Apple's current policies concerning iOS.  With a rewrite, we have complete freedom to choose a less restrictive Free Software/Open Source license.
> > The apps could either be reimplemenation/cloning of our current games, or entirely new educational activities that fit with our established mission.  They must be recognizable as Tux4kids software via shared logos and (of course) Tux himself.
> > Technical options include:
      * _HTML5 plus scripting language plus cross-mobile-platform development framework:_  This has the advantages of rapid development and immediate compatibility with both leading smartphone/tablet platforms. Few FOSS-compatible systems of which we are aware are:
        * HTML5/Phonegap/Javascript
        * MOAI/Lua, +/- C++.
      * _Java/Android:_ The Java language is extremely well supported and documented, as are both the Android and Java delivery platforms.  Straight Java allows programs to be developed as installed applications, as browser-based applets, and as WebStart applications that can be very easily installed over the Web.  These are all strong advantages for us. Furthermore, the same Java code can be used as the basis of a native Android app. The biggest disadvantage of Java is that it does not directly lead to an app usable on iOS.
      * _HaXe NME:_ The Tuxmath mobile app has been built on the open-source NME framework (MIT license), which provides cross-platform support for Android, iOS, HTML, and Flash among others out of box. The development is supported on Windows, Linux and Mac platforms. HaXe will look very familiar if you are coming from an AS3 background.

  * Prerequisites:
    * Knowledge of either HaXe/NME or HTML5/Javascript/Phonegap or MOAI/Lua/C++.
    * Alternatively, knowledge of Java and Android Development.
    * Prior game(s) written from scratch strongly preferred.
    * Knowledge about UX/UI designing.
    * Knowledge of working with different resolutions.
    * Lots of Creativity.
    * Git knowledge is a must.

_**Mentor:**_ aaditya025@gmail.com


**Note**: All names listed are possibly mentor for this year for particular projects however can be swap according the phase of project duration and students requirement.