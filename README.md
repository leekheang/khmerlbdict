# Khmer LineBreaking Dictionary

The aim of this project is to produce a frequency based wordlist for line and word breaking
Khmer language. This will then be used in ICU (if they accept it).

Sources are:

* seafreq.txt. Taken from the SEALang Khmer frequency based wordlist [http://sealang.net/project/list/]
* villages.txt. A list of all village and region names
* places.txt. Language, script, territory and exemplar city names taken from CLDR.
* names.txt. Various first and last names.

The files are edited to remove bad data, for example villages called 'number1'.

A program then calculates the log frequencies needed for CLDR and adds equivalences for bad spellings.
This will mean badly spelled data that is hard to spot will break correctly and it will be up to a
spelling checker to sort that mess out.
