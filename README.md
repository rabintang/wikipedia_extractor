wikipedia_extractor
===================

This is a multithreaded version of the original WikipediaExtractor


Usage
===================

$ ./WikiExtractor.py -h
usage: WikiExtractor.py [-h] [-w] [-b n[KM]] [-c] [-l] [-s] wikidump outputdir

Multithread Wikipedia Extractor:
    
Extracts and cleans text from Wikipedia database dump and stores output in a
number of files of similar size in a given directory.
Each file contains several documents in the format:
    
	<doc id="" url="" title="">
        ...
        </doc>

positional arguments:
  wikidump              XML wiki dump file
  outputdir             output directory

optional arguments:
  -h, --help            show this help message and exit
  -w, --overwrite       Overwrite existing output dir
  -b n[KM], --bytes n[KM]
                        put specified bytes per output file (default is 25M)
  -c, --compress        compress output files using bzip
  -l, --links           preserve links
  -s, --sections        preserve sections
