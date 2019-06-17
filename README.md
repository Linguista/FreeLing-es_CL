# FreeLing-es_CL
# Scott Sadowsky
# http://sadowsky.cl

**Linguistic resources for adapting FreeLing to Chilean Spanish**

[FreeLing](https://github.com/TALP-UPC/FreeLing) in an open source tool for performing natural language processing on a variety of languages. Among other things it lemmatizes, chunks and morphologically tags orthographic text.

This repository contains a series of resources I've developed to make FreeLing perform better with Chilean Spanish. To use, clone the main FreeLing repository, clone this repository, copy this repository's files into the FreeLing directory, and then make and compile FreeLing.

There are various README files throughout the file tree. These explain different options that users have when copying over files. In particular, there are two different sets of dictionary files for auxiliary verbs, main verbs and pronouns -- one with a specific tag value to mark voseo forms (not included in the main FreeLing repo, as including this information was not foreseen by the designers of the EAGLES tagset and is therefore considered non-standard), and one without (included in the main FreeLing repo's Chilean Spanish data). 
