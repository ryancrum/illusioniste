# Illusioniste

A (very) thin wrapper over im4java, a wrapper over ImageMagick's command-line utilities. This is literally nothing more than a small macro.

## Usage

Add The following to your project.clj
    [illusioniste "1.0.1-SNAPSHOT"]

    (ns example.core
      (:require [illusioniste]))

    (illusioniste/transform-image image-byte-array
      (rotate 90.0)
      (crop 140 100)
      (resize 80 80)) ;; returns jpeg byte array rotated 90 degrees,
                      ;;   cropped to 140x100
                      ;;   and subsequently resized to 80x80

## Todo

* Some helpers to get images into and out of byte-arrays
* Support more than simple convert calls (composite, etc.)

## License
Copyright &copy; 2011-2013 Ryan Crum, Justin Tirrell and Renaud Tircher.
Distributed under the Eclipse Public License. See LICENSE.
