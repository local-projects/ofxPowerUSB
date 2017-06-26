# ofxPowerUSB

Minimal command line driven addon to control [PowerUSB Basic](http://www.pwrusb.com/index.html)

Lets you control external power switch from inside oF.

Only included OSX version, but Win should be the same.

# Setup

1. Put libpowerusb.dylib & pwrusbcmd in binary app folder.
2. Add libpowerusb.dylib to the Resource folder. In xcode, go to 'BuildPhases>Copy files' and add libpowerusb.dylib.

![setup image](https://github.com/local-projects/ofxPowerUSB/blob/master/readme_images/Screen%20Shot%202017-06-26%20at%2010.44.41%20AM.png?raw=true)

# Notes
* The expected paths for the dylib image behaved differently on different OSX systems.
* Failed to integrate their source code because of internal NSExceptions from their dynlib.
* Removed pause to enter on pwrusbcmd to prevent getting stuck when not connected.

