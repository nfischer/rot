rot
===

A simple rot13 encrypter/decrypter with some testing to see if a file is encrypted or decrypted.

Usage
===
This is a bash script that can be used to encrypt/unencrypt files with a simple rot 13 rotation.
Because this is a bash script, you only need to give it executable permission.
	$ chmod +x rot
	$ chmod 755 rot

Because this is a rotation by 13, one command will both encrypt <b>and</b> unencrypt.
	$ ./rot someFile.txt

If you type "unencrypted" on the top line of your file, this script will also tell you when your file is encrypted or unencrypted. Additionally, this feature may also work with html5 files.

Multiple files
---
You can pass multiple files as arguments and this script will encrypt each file with the algorithm.
	$ ./rot firstFile secondFile

Stdin
---
You can also encrypt input from stdin (works in conjunction with files as arguments as well).
	$ cat someFile | ./rot
	$ echo "Hi" | ./rot firstFile secondFile

