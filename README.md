mbib
====

A python script for manipulating bibtex entries in tex and bibtex files.

* List all bibkeys cited in a LaTeX source.
* Detection of **unreferenced** or **uncited** keys in a LaTeX source.
* Generation of BibTeX file from LaTeX source.

Usage
-----

Too get some help:
~~~
$ mbib -h
~~~

You can have a try on the provided example.
~~~
$ mbib exemple.tex  # bibkeys cited in tex file
Anyone1996
Grandpa1923
Nobody
Someone1996

$ mbib -u exemple.tex  # bibkeys cited but not defined in bibfile
Anyone1996

$ mbib -n exemple.tex  # bibkeys not cited but defined in bibfile
Anyone1997             

$ mbib -n -b exemple.tex  # same as above in bibtex style
@misc{Anyone1997,
       author = {Anyone Jr.},
       title = {My book},
       year = {1997}}
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
