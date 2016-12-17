# Release Notes
## General

## Version 0.2.5
Released: Work in Progress
### What's new?
Added the ability to perform "once-off" exports of user selected gThumb catalogs. This is useful for bringing one or more albums on a USB key while visiting friends or family. It is also useful to quickly give someone a copy of the photos of a specific event.

### Resolved issues
* User manual is nearly complete.
* Details on the configuration file are complete.
* Resolved issue where backups of catalog files were processed as well.

### Known issues
* Program does not properly handle the situation whereby the user specifies more than one parameter, e.g. using "-s" and "-e" at the same time. The program should never be run with both these options at the same time, but it would be nice if the program would output a message to that extent, rather than starting excution.

### Limitations
* The program requires that there is one (1) source directory containing the actual photos.
* The program has not been tested with nested libraries and nested catalogs.

## Version 0.2.1
Released: 6 December 2016

### What's new?
The configuration file has a new variable called "SKIPYEARLIBS". When its value is set to "yes", the library selection list will not show libraries whose names are individual years.

### Resolved issues
* There was an issue whereby library names containing spaces would not display properly and as a result could not be synchronised. This has now been resolved.

### Known issues
User manual still needs to be written. Limited information is available in the Github repository around the general use of gthumb2tv. Descriptions are available in the gthumb2tv.cfg file to assist users getting started.

### Limitations
* The program requires that there is one (1) source directory containing the actual photos.
* The program has not been tested with nested libraries and nested catalogs.
