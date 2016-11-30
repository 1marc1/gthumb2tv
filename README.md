# gthumb2tv
Software that allows you to export gThumb libraries and catalogs for viewing on an external device, such as a TV.
## What is it?
Most modern TVs have the ability to display images stored on a USB stick. Also, most media center solutions (such as Kodi) have the ability to show images. If you manage your photo albums with gThumb on your computer, you can then use this software export your gThumb libraries and catalogs for viewing on your TV.

gthumb2tv is a bash script that uses rsync to synchronise your photos to another location (e.g. a USB stick, NAS, etc). It then synchronises your gThumb catalogs. In doing so, it is effectively also creating a backup for you.
It creates a directory structure based on your catalog names and fills these directories with symbolic links to the original images. This way, your "Smart TV" can actually look smart by allowing you to browse through your photo albums. If you use Kodi (or another Media Center) you can point it to the source of your photos and allow your Media Center to drive your slide shows.

## Why this software?
People are making more and more photos thanks to modern technology. gThumb provides an excellent way to organise your photos in albums. Now that you have come this far, wouldn't it be great to also show off your photo albums to your friends and relatives from the comfort of your sofa without having to pass the laptop around? Or: have a slideshow of your photographic artwork playing on your TV while you are having a party.

## The latest version
The latest version, including documentation can be downloaded from https://github.com/1marc1/gthumb2tv.

## Installation and usage
Please see the INSTALL file bundled with this package for details on installing this software.
Please see the "gthumb2tv User Manual" file for full details on how to use this software.

## Licensing
Please see the LICENSE file bundled with this package for licensing details.

## Contact
Comments, requests for improvements, etc. are welcome via https://github.com/1marc1/gthumb2tv/issues.
