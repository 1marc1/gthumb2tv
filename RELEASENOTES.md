# Release Notes
## General
The general flow of gthumb2tv is as follows:
* rsync photos from source to destination
* let user select the library to process
* compare catalog file names between source and destination
  * if a catalog is found in the source, which does not exist in the destination:
    * copy the catalog file from source to destination
    * create directory for symlinks belonging to this catalog
    * create the symlinks in the directory for this catalog
  * if a catalog is found in the destination, which does not exist in the source:
    * delete the directory for symlinks belonging to this catalog at the destination
    * delete the catalog file at the destination
  * if a catalog is found that exists in the source and destination:
    * if source and destination are identical:
      * do nothing
    * else
      * delete the catalog at the destination
      * delete the directory for symlinks belonging to this catalog
      * copy the catalog file from source to destination
      * create directory for symlinks belonging to this catalog
      * create the symlinks in the directory for this catalog
* create a special "Latest Albums" album.

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
