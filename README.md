Rot13
=====

A simple rot13 encrypter/decrypter. Why would you ever use this? Only if you
were taking CS 35L at UCLA and wanted to test if your rot13 project
worked... Or if you ever need super simple encryption to get a file past
someone who knows nothing about computers.

But hey, at least you *look* like you care about security.

Usage
-----

Encrypt and unencrypt your files with the same command!

```
$ ./rot someFile.txt
```

As an added bonus, if you type "unencrypted" on the top line of your file,
this script will also tell you when your file is encrypted or unencrypted.

Multiple files
--------------

You can pass multiple files as arguments and this script will encrypt each
file with the algorithm.

```
$ ./rot firstFile secondFile
```

Stdin
---

You can also encrypt input from stdin (works in conjunction with files as
arguments as well).

```
$ cat someFile | ./rot
$ echo "Hi" | ./rot firstFile secondFile
```

So what's this really about?
----------------------------

Ok, you caught me. Really, I wanted an excuse to practice shell scripting
and learn about processing standard input (without hanging if no input is
supplied). And that's harder than it seems actually.

The rot13 part was a fun bonus, since it was easier than teaching
a non-CS major how to do rot13 within vim (it's `ggg?G` by the way). And
rot13 is just fun in general.
