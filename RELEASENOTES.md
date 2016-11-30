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

## Version 0.2
Released: 1 December 2016

### What's new?
Complete rewrite of the original version. This version is the first version that is publicly available.

### Resolved issues
* Added many more functions and remarks inside the code to make the program more easily readable.
* Added more detail to the log.
* Removed limitation of having to start catalog names with three numbers.

### Known issues
None.

### Limitations
* The program requires that there is one (1) source directory containing the actual photos.

## Older than version 0.2
The original and initial version of this software was built in July 2016. This version was never publicly released. Between then and the release of first publicly available version (version 0.2), a number of bug fixes and updates took place.
