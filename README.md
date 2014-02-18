PLAINTAG
========

Plaintext-based file tagging.

SYNOPSIS
--------

    plaintag [options] list     <tag>  [<tag>...] -- list files tagged with all of these tags
    plaintag [options] listany  <tag>  [<tag>...] -- list files tagged with any of these tags
    plaintag [options] show     <file>            -- list tags associated with a file
    plaintag [options] tag[+|-] <file> [<tag>...] -- add, remove or overwrite a tag list associated with a file

DESCRIPTION
-----------

_plaintag_ is a general purpose tagging program written with
simplicity in mind. The whole database is just a directory (by default
in _~/.plaintag_, may be changed with an _-d_ option) with a single
file for each tag. Each of them contains a list of absolute paths to
files tagged with it. They can be easily modified using tools such as
`mv`, `sed`, `grep` or `vim`.

The bundled script _plaintag-gui_ allows easy tag manipulation. Just
pass a file as an argument for it to show an input box with the
current tags for that file. Personally I use it with `sxiv` image
viewer.

OPTIONS
-------

*   __-d__ _directory_

    specify a custom database

EXAMPLE
-------

    plaintag -d ~/image_tags tag pikachu.jpg pokemon yellow mouse thunder

PLANNED FEATURES
----------------

* more comprehensive readme
* better GUI

DEPENDENCIES
------------

* `zsh`
* `zenity` for GUI

AUTHOR
------

Wojciech 'vifon' Siewierski < wojciech dot siewierski at gmail dot com >

COPYRIGHT
---------

Copyright (C) 2014  Wojciech Siewierski

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program.  If not, see <http://www.gnu.org/licenses/>.
