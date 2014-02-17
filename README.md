wikipedia_extractor
===================

This is a multithreaded version of the original WikipediaExtractor

Usage
===================

$ ./WikiExtractor.py -h<br/>
usage: WikiExtractor.py [-h] [-w] [-b n[KM]] [-c] [-l] [-s] wikidump outputdir

Multithread Wikipedia Extractor:
    
Extracts and cleans text from Wikipedia database dump and stores output in a
number of files of similar size in a given directory.
Each file contains several documents in the format:
    
	<doc id="" url="" title="">
        ...
	</doc>

positional arguments:<br/>
&emsp;wikidum&emsp;&emsp;XML wiki dump file<br/>
&emsp;outputdi&emsp;&emsp;output directory

optional arguments:<br/>
&emsp;-h,&emsp;--help&emsp;&emsp;show this help message and exit<br/>
&emsp;-w,&emsp;--overwrite&emsp;&emsp;Overwrite existing output dir<br/>
&emsp;-b n[KM],&emsp;--bytes n[KM]&emsp;&emsp;put specified bytes per output file (default is 25M)<br/>
&emsp;-c,&emsp;--compress&emsp;&emsp;compress output files using bzip<br/>
&emsp;-l,&emsp;--links&emsp;&emsp;preserve links<br/>
&emsp;-s,&emsp;--sections&emsp;&emsp;preserve sections
