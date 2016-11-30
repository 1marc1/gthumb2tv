# gthumb2tv
## Prerequisites
The following is a list of additional software that is required in order to successfully run gthumb2tv. I have listed the versions that are installed on my Ubuntu 14.04 machine as I know these versions work. If you have a different version of the software from that listed below, it is not to say that your version does not work.
* gthumb 3.2.7
* convert (available in ImageMagick 6.7.7-10 2016-06-01 Q16)
* identify (available in ImageMagick 6.7.7-10 2016-06-01 Q16)
* rsync 3.1.0
* comm (GNU coreutils) 8.21
* diff (GNU diffutils) 3.3
* bash 4.0 or later

## Installation
After you have downloaded the latest version (see README.md for download location), extract the ZIP file to a temporary location. You will find the following files in the installation package:
* gthumb2tv.cfg   <--- configuration file
* gthumb2tv       <--- program file

We need to make the program file executable and place it in a location that is convenient for you to execute. The configuration file should be placed in the root of your home directory.

For example:
~~~~
1marc1@myhost:/tmp$ ls -l
-rw------- 1 1marc1 1marc1   131 Nov 25 17:56 gthumb2tv.cfg
-rw------- 1 1marc1 1marc1 32011 Nov 25 17:56 gthumb2tv
1marc1@myhost:/tmp$ sudo chown 1marc1:1marc1 gthumb2tv.cfg gthumb2tv
1marc1@myhost:/tmp$ chmod 744 gthumb2tv
1marc1@myhost:/tmp$ ls -l
-rw------- 1 1marc1 1marc1   131 Nov 25 17:56 gthumb2tv.cfg
-rwxr--r-- 1 1marc1 1marc1 32011 Nov 25 17:56 gthumb2tv
1marc1@myhost:/tmp$ mv gthumb2tv.cfg ~
1marc1@myhost:/tmp$ sudo mv gthumb2tv /usr/local/bin
~~~~

## Configuration
For details on configuring and using gthumb2tv see the user manual.
