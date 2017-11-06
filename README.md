# bigflies

Command-line utilities for dealing with big files.

So far, this contains only a simplified python reimplementation of
[`wcl`](https://github.com/MyLifeLabs/wcl).

## wcl

`wcl` is `wc -l` for the impatient. It counts the number of lines in a
collection of files and displays an estimate as it progresses.

It is recommended if you need is an estimate of the number of lines in
your files. You can just launch `wcl` and interrupt it once the
estimate seems to stabilize. Here's an example of `wcl` running on 3
files:

```
$ wcl bigdata-part1.dat bigdata-part2.dat bigdata-part3.dat
 11% estimate: 443,486,924 lines
```

Later, when done:

```
$ wcl bigdata-part1.dat bigdata-part2.dat bigdata-part3.dat
443,486,884
$
```
