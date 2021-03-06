Introduction
------------
How to build the LinkM library and example code.

Details
-------
The build process for all LinkM software except the Processing apps is expected to be done entirely from the command-line using standard free Unix-like tools such as "make" and "gcc".

There is a build_all_host.sh script that will build the host-side code on all OS platforms.

Host code dependencies:
-----------------------
- The Java library in "java_host" depends on the C library in "c_host"
- The C library in "c_host" depends on library in "bootloadHID/commandline"

On Mac OS X you will need the following free tools:

- XCode - http://developer.apple.com/technologies/xcode.html
- libusb - "sudo port install libusb-legacy libusb" (port is available from http://macports.org/ )

On Windows you will need the following free tools:

- MinGW - http://www.mingw.org/
- MSYS - http://www.mingw.org/wiki/MSYS
- zip - http://stahlworks.com/dev/index.php?tool=zipunzip
- Java JDK - http://java.sun.com/javase/downloads/widget/jdk6.jsp

On Ubuntu Linux you will need the following free tools:

- build-essential - 'sudo apt-get install build-essential'
- libusb - 'sudo apt-get install libusb libusb-dev'
- Sun JDK - 'sudo add-apt-repository "deb http://archive.canonical.com/ lucid partner" && sudo apt-get update && sudo apt-get install sun-java6-jdk'

