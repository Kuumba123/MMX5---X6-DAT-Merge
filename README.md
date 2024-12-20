# MegaMan X5/X6 DAT Merge
this program reads a text file witch lists files to be merged in to 1 file with archive format used in X5/X6 .

using this program is pretty simple just put the script in the same folder as the text file + data files then do the following
```
python datMerge.py <input_textFileList> <output_fileName> [-d]
```
The `-d` flag is optional is simply adds in a dummy header sector if amount of entries is less than or equal to 0x100.
The format for the text file is simple , a line starting with `//` is a comment and anything other than that is a file to be add as an entry. 
Entries can be combined by simply using a `,` to merge the 2 or more files.