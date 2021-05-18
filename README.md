Font Dozenalizer
================

Add a ↊ [(turned digit two U218A)](https://unicode-table.com/en/218A/) and a ↋ [(turned digit
three U218B)](https://unicode-table.com/en/218B) glyph to a given TrueType font by
rotating the existing glyphs for two and three by 180 degrees and adding them at
the right unicode points.

Installation
------------

Make sure you have [Python 3](https://www.python.org/downloads/) installed on your computer.
Then clone or download the repository and then install the dependencies by running the following command on a commandline.

```bash
python3 -m pip install -r requirements.txt
```

Or in case you prefer a dedicated virtual python environment you can do

```bash
source setup.sh
```

Usage
-----

It's a standard Python commandline utility which you can run from any commandline as follows.

```
$ python3 addglyphs.py -h
usage: addglyphs.py [-h] [--ttx] [--no-ttx] inputfile outputfile

Add a turned two (U218A) and a turned three (U218B) glyph to the given TrueType font.

positional arguments:
  inputfile   file name of the input font
  outputfile  file name of the output font

optional arguments:
  -h, --help  show this help message and exit
  --ttx       also dump a ttx file of the result
  --no-ttx
```

So for example

```
$ python3 addglyphs.py Arial.ttf ArialEnriched.ttf
```

will read an existing file called `Arial.ttf` and produce a new file named `ArialEnriched.ttf` containing the additional dozenal glyphs.

