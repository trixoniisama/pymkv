# pymkv

pymkv is a Python wrapper for mkvmerge and other tools in the MKVToolNix suite. It provides support for muxing,
splitting, linking, chapters, tags, and attachments through the use of mkvmerge.

## About pymkv
pymkv is a Python 3 library for manipulating MKV files with mkvmerge. Constructing mkvmerge commands manually can
quickly become confusing and complex. To remedy this, sheldonkwoodward decided to write this library to make mkvmerge more
scriptable and easier to use. Please open new issues for any bugs you find, support is greatly appreciated!

## This fork
Adapted to work on Linux systems properly. Added *track delay* feature and changed up some other things.
For example, if no *title* is specified in **`MKVFile()`**, there won't be one in the output file, unlike the original project which would keep the title of the pre-existing file if it existed. Now in order to keep the title, you need to specify *title="keep"*.

## Installation
mkvmerge must be installed on your computer, it is needed to process files when creating MKV objects. It is also
recommended to add it to your $PATH variable but a different path can be manually specified. mkvmerge can be found
and downloaded from [here](https://mkvtoolnix.download/downloads.html) or from most package managers.

To install this pymkv fork, use the following commands:

```
git clone https://github.com/trixoniisama/pymkv.git
cd pymkv
pip install -e .
```

## Documentation
The current documentation for pymkv is lacking.
Still, most of what needs to be known can be found here : [DOCUMENTATION](https://pymkv.shel.dev)
