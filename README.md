# electron-sample

Electron simple sample project.


## Requirements

* [Node.js](http://nodejs.org/)


## Quick Start

1) go to the root folder of this project on command line

``` bash
$ cd /PROJECT-ROOT
```

2) install dependency files

``` bash
$ npm install
```

3) run the application

``` bash
$ npm start
```


## Packaging for MacOS and Windows (x86_64)

### Building Windows apps from non-Windows platforms

Building an Electron app for the Windows target platform requires editing the `Electron.exe` file.
Currently, Electron Packager uses [node-rcedit](https://github.com/atom/node-rcedit) to accomplish
this. A Windows executable is bundled in that Node package and needs to be run in order for this
functionality to work, so on non-Windows host platforms, [Wine](https://www.winehq.org/) 1.6 or
later needs to be installed. On OS X, it is installable via [Homebrew](http://brew.sh/).

``` bash
$ npm run bundle.mac
```

``` bash
$ npm run bundle.windows
```

You can also run electron-packager from the command line using the following basic form:

``` bash
$ electron-packager <sourcedir> <appname> --platform=<platform> --arch=<arch> [optional flags...]
```

### Reference:

https://github.com/electron-userland/electron-packager