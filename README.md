# git-analytics

git analysis tools, created and maintained by Tech DNA.


## Requirements

* A Unix-like system -- tested on Linux, OSX and WSL2
* Recent Python 3.x
* Recent SQLite3

## Installation

Ensure key components are at their minimum version:

* Python 3.7 or newer 
* SQLite 3.24 or newer
* git 2.0 or newer

## git-who Usage

```
# change directory to your top source directory
# it can be a top directory with git checkouts in subdirectories
cd /path/to/my/code

# collect the stats -- this may take some time
git-who init

# output stats
git-who stats

# output for a particular directory
git-who stats some/component

# output stats in csv format
git-who --csv stats

# statistics are stored in a hidden sqlite file
ls .git-who.sqlite3

# you can open it, and explore its contents
sqlite3 .git-who.sqlite3

```

## Authors

* Martin Langhoff - martin.langhoff@tech-dna.net / martin.langhoff@gmail.com - creator and maintainer

## Copyright and License

Copyright Tech DNA LLC 2021

git-analytics is licensed under GPLv2.
