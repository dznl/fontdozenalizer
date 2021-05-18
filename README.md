Font Dozenalizer
================

Add a turned two [(U218A)](https://unicode-table.com/en/218A/) and a turned
three [(U218B)](https://unicode-table.com/en/218B) glyph to a given TrueType font by
rotating the existing glyphs for two and three by 180 degrees and adding them at
the right unicode points.

Installation
------------

Clone the repository and install the dependencies.

### Virtual environment

```bash
source setup.sh
```

### Global environment

```bash
python3 -m pip install -r requirements.txt
```

Usage
-----


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

