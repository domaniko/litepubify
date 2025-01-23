# litepubify

**litepubify** is a program to download stories from literotica.com and convert them to the .epub format for e-book reader use, etc. It can fetch a single story or an entire series.

litepubify is a command line program, written in python (no external dependencies, python version 2.6, 2.7 or >=3)

Sample usage:

`$ python litepubify.py 'http://www.literotica.com/s/my-favorite-story'`

All options:
```
usage: litepubify.py [-h] [-a AUTHOR] [-t TITLE] [-o FILENAME] [-s]
                     [--noteaser] [--noimages] [-v] [-d] [--silent]
                     [--disk-cache-path PATH]
                     url [url ...]

positional arguments:
  url                   URL of the story, or one of the stories in the series

optional arguments:
  -h, --help            show this help message and exit
  -a AUTHOR, --author AUTHOR
                        override the author in the epub metadata
  -t TITLE, --title TITLE
                        override the title in the epub metadata and default
                        file name
  -o FILENAME, --output FILENAME
                        set output file name (optional, otherwise story title
                        is used)
  -s, --single          do not attempt to download the entire series (if it is
                        a series) but just this one story
  --noteaser            do not include the one line teaser in the table of
                        contents
  -v, --verbose         output more information
  -d, --debug           output debug information
  --silent              suppress informational output
  --disk-cache-path PATH
                        Path for the disk cache (this is normally not needed).
                        If this option is specified, downloaded websites are
                        cached in a file and loaded in subsequent runs (when
                        this option is used again with the same path). This is
                        mainly useful for testing, to avoid repeated
                        downloads.
```


Written by hoelty, revised by mueslimak3r, license: CC0.

