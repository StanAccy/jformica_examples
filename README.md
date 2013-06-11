Self contained eclipse project. Uses usb4java for JSR80 implementation. 

Windows:
- use Zadig to install libusbK for ant stick
- see:  https://github.com/libusbx/libusbx/wiki/Windows-Backend#wiki-How_to_use_libusbx_on_Windows

Linux:
- make udev rule for ant-stick
- see: http://kayahr.github.io/usb4java/faq.html

OSX:
- should work, but not sure if there are additonal steps. 

Common:
- import project dir into eclipse e.g jformica_java
- fix JRE/JDk setup (see section below)
- compile and run

Fix JRE:
- right click imported project
- click properties
- When dialog appears, click 'Java Build Path'
- click 'JRE system library'
- click edit
- select an execution environment that exists on your system (Workspace default?)

TROUBLESHOOTING:

Here are some errors and solutions that have been reported.

Windows:

EXCEPTION_ACCESS_VIOLATION in libusb usbi-read :

Try updating Zadig or installing the latest libusk from: http://libusbk.sourceforge.net/UsbK3/index.html


Where is the source?

- source code for usb4java : https://github.com/kayahr/usb4java
- source code for jformica: https://github.com/cowboy-coders/JFormica/tree/jformica_branch
