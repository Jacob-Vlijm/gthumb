# gThumb

An image viewer and browser utility for the GNOME environment.
More information can be found at https://wiki.gnome.org/Apps/Gthumb.

## Features

 * gThumb is an image browser

   + Browse your hard disk showing you thumbnails of image files.
   + Thumbnails are saved in the same database used by Nautilus so you
     don't waste disk space.
   + Automatically update the content of a folder.
   + Copy, move, delete images and folders.
   + Bookmarks of folders and catalogs.

 * gThumb is an image viewer

   + View single images (including GIF animations).  Supported image
     types are: BMP, JPEG, GIF, PNG, TIFF, TGA, ICO, XPM.
   + Optional support for RAW and HDR (high dynamic range) images.
   + View EXIF data attached to JPEG images.
   + View in fullscreen mode.
   + View images rotated, flipped, mirrored.

 * gThumb is an image organizer

   + Add comments to images.
   + Organize images in catalogs, catalogs in libraries.
   + Print images and comments.
   + Search for images on you hard disk and save the result as a catalog.
     Search criteria remain attached to the catalog so you can update it
     when you want.

 * gThumb is an image editor

   + Change image hue, saturation, lightness, contrast and adjust colors.
   + Scale and rotate images.
   + Save images in the following formats: JPEG, PNG, TIFF, TGA.
   + Crop images.
   + Red-eye removal tool.

 * gThumb is an advanced tool

   + Import images from a digital camera.
   + Slide Shows.
   + Set an image as Desktop background.
   + Create index image.
   + Rename images in series.
   + Convert image format.
   + Change images date and time.
   + JPEG lossless transformations.
   + Find duplicated images.

## Extensions

  gThumb has a plug-in system for extensions. Some standard features
  are implemented as extensions and are supplied with the standard
  distribution. Users may write (and share) additional extensions.

  See https://wiki.gnome.org/Apps/Gthumb/extensions for details.

## Licensing

  This program is released under the terms of the GNU General Public
  License (GNU GPL), either version 2 of the License, or (at your option) any
  later version.

  You can find a copy of the license in the file COPYING.

## Compiling

  In order to build this program you need GNOME 3, with the development tools installed properly.
  The following is the detailed list of libraries you need:

  * glib >= 2.38.0
  * gtk  >= 3.16
  * libpng
  * zlib
  * libjpeg
  * gsettings-desktop-schemas

  While not mandatory, the following libraries greatly increase gThumb's basic usefulness:

  * exiv2: embedded metadata support;
  * gstreamer, gstreamer-plugins-base, gstreamer-video: audio/video support;
  * libtiff: tiff writing support.

  Other optional libraries:

  * libraw: some support for RAW photos;
  * librsvg: display SVG images;
  * libwebp: display and save WebP images;
  * lcms2, colord: color profile support;
  * champlain, champlain-gtk: view the place a photo was taken on a map;
  * clutter, clutter-gtk: enhanced slideshow effects;
  * libsoup, json-glib, webkit2gtk, libsecret: upload images to and download images from some web services such as facebook, flickr;
  * brasero: write images and comments to CDs;
  * bison, flex: web albums.

## Download

  * Tar archives can be found here:

    http://ftp.gnome.org/pub/GNOME/sources/gthumb

  * You can download and compile the latest development version using the
    following commands:

        git clone https://gitlab.gnome.org/GNOME/gthumb.git
        cd gthumb
        meson build
        ninja -C build
        sudo ninja -C build install

   More development information is available at
   https://wiki.gnome.org/Apps/Gthumb/development