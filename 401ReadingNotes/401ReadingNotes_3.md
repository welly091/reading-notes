# [Reading and Writing Files in Python](https://realpython.com/read-write-files-python/)

Open a file
```file = open(myfile.txt, 'r')```

Close a file
```file.close()```

Second arguments in open():

|Character|Meaning|
|---------|-------|
|'r'|Open for reading(default)|
|'w'|Open for writing, truncating(overwriting) the file first|
|'rb' or 'wb'|Open in binary mode(read/write using byte data)|

We usually use try-finally for handling files:

```
reader = open('dog_breeds.txt', 'r')
try:
    # Further file processing goes here
finally:
    reader.close()
```
However, sometimes it's easy to forget to close the file. Therefore, ```with``` is introduced.

```
with open('dog_breeds.txt', 'r') as reader:
```

## Reading and Writing Opened Files
|Method|What It Does|
|---|---|
|.read(size==1)|This read from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.|
|.readlin(size=-1|This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.|
|.readlines()|This reads the remaining lines from the file object and returns them as a list.|
