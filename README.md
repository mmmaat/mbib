mbib
====

A python script for manipulating bibtex entries in tex and bib files.

* List all bibkeys cited in a LaTeX source.
* Detection of unreferenced or uncited keys in a LaTeX source.
* Generation of BibTeX file from LaTeX source.

Usage
-----

Basic usage is shown on the provided (example.tex) and (example.bib).

~~~
$ mbib -h               # get some help !
$ mbib example.tex      # list the keys cited in the tex file
$ mbib -u example.tex   # list the keys undefined in the bib file
$ mbib -n example.tex   # list the not cited in the tex file
~~~

Licence
-------

Copyright (C) 2015 Mathieu Bernard

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see (http://www.gnu.org/licenses/).
