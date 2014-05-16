# Arduino Serial Monitor Permission Fix for OSX

When developing applications for the arduino on OSX you might have encountered the dreadful issue of:

"Can't open /dev/tty.XXXXX Resource is busy" even though no other application was accessing the Arduino at the same time

To fix this issue the following folder /var/lock needs to be world read+writable. This AppleScript will perform the necessary
shell commands to fix the issue. That's the reason why it requires administrative privileges.

Tested on: OSX Mavericks 10.9.3
Tested with: Arduino Uno R3 / Arduino Yun
