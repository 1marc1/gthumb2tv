# gthumb2tv
## Installation
After you have downloaded the latest version (see README.md for download location), extract the ZIP file to a temporary location. You will find the following files in the installation package:
* gthumb2tv.cfg   <--- configuration file
* gthumb2tv       <--- program file

We need to make the program file executable and place it in a location what is convenient for you to execute. The configuration file should be placed in the root of your home directory.

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
Now we need to update the configuration file.
