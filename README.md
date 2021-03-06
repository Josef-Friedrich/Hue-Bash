[![Build Status](https://travis-ci.org/Josef-Friedrich/Hue-shell.svg?branch=master)](https://travis-ci.org/Josef-Friedrich/Hue-shell)

`Hue-shell` is a collection of shell scripts to control the Hue lamps
from Philips.

```
                    _________________________
                   /                         \
                  +    ___________________    +
                  |   /                   \   |                      .
                  |   + _$ hue set 1 --on  +  |            .    +    ,
                  |   |                    |  |             \   '   /
  ,+.             |   +                    +  |              ` ,+. '
 (   )            |   \___________________/   |           +-+ (   ) +-+
  \ /     -->     +  /+\               _      +     -->        \ /
 _+=+_             \_________________________/                _+=+_
+_____+              !______________________!                +_____+

```

It is designed for embedded operating systems with very
limited resources (successfully tested on the old and outdated wifi
router "Linksys WRT54GL").

`Hue-shell` runs on many shells (sh, dash,
ash, bash) and many UNIX operating systems (Linux, MacOS X, FreeBSD,
OpenWrt). `Hue-shell` works well in a small BusyBox environment. Out
of the box `Hue-shell` runs on many single-board computer like
Raspberry Pi, Cubieboard, BeagleBone etc.

# Installation

```sh
sudo sh -c "OPT=install; $(curl -fksSkL http://raw.github.com/Josef-Friedrich/Hue-shell/master/install.sh)"
```

To install `Hue shell` manually please read the [documentation on the project page](http://josef-friedrich.github.io/Hue-shell/installation.html).

# Features

```
              .--------------.
           ___|  _  _  _  _  |_________________
          /   |  || || || ||_|___             /;      Hue-shell runs on
         /.--------------.      /|___        //     many single-board computer
        / |  _  _  _  _  |     / ___ \      //     like Raspberry Pi,
       /  |  || || || || |____/ ___ \(\)   //     Cubieboard, BeagleBone etc.
      /   |  || || || || |    | /  \(\)   //
     /    |______________|____|/   (\)   //
    / _                                 //
   / (\) Raspberry Pi                  //
  /___________________________________//
  `-----------------------------------'
```

* Versatile basic command `hue set ...`
* Requires very little resources, runs in small UNIX environments
* Moving light scenes to create a ambient and decent atmosphere (`huescene-breath` `..-pendulum`, `..-sequence`)
* Background services to detect reachable bridge and blubs.

For further documentation please visit the [project site](http://josef-friedrich.github.io/Hue-shell/):

http://josef-friedrich.github.io/Hue-shell/

# Commands

## Basic commands

* [hue](http://josef-friedrich.github.io/Hue-shell/docs/hue.html)

## Load commands

* [hueload-default](http://josef-friedrich.github.io/Hue-shell/docs/hueload-default.html)
* [hueload-random](http://josef-friedrich.github.io/Hue-shell/docs/hueload-random.html)
* [hueload-scene](http://josef-friedrich.github.io/Hue-shell/docs/hueload-scene.html)

## One color commands

* [huecolor-basic](http://josef-friedrich.github.io/Hue-shell/docs/huecolor-basic.html)
* [huecolor-recipe](http://josef-friedrich.github.io/Hue-shell/docs/huecolor-recipe.html)

## Scene commands

* [huescene-breath](http://josef-friedrich.github.io/Hue-shell/docs/huescene-breath.html)
* [huescene-pendulum](http://josef-friedrich.github.io/Hue-shell/docs/huescene-pendulum.html)
* [huescene-sequence](http://josef-friedrich.github.io/Hue-shell/docs/huescene-sequence.html)

## Service commands

* [hueservice-detect-bridge](http://josef-friedrich.github.io/Hue-shell/docs/hueservice-detect-bridge.html)
* [hueservice-detect-lights](http://josef-friedrich.github.io/Hue-shell/docs/hueservice-detect-lights.html)

## Management commands

* [hue-manager](http://josef-friedrich.github.io/Hue-shell/docs/hue-manager.html)
