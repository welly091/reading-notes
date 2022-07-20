# [Reading and Writing Files in Python](https://realpython.com/read-write-files-python/)
Take a quiz here [Quiz!!!](https://realpython.com/quizzes/read-write-files-python/)

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
|'a'|Append a file|

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

## Reading Opened Files
|Method|What It Does|
|---|---|
|.read(size==1)|This read from the file based on the number of size bytes. If no argument is passed or None or -1 is passed, then the entire file is read.|
|.readlin(size=-1|This reads at most size number of characters from the line. This continues to the end of the line and then wraps back around. If no argument is passed or None or -1 is passed, then the entire line (or rest of the line) is read.|
|.readlines()|This reads the remaining lines from the file object and returns them as a list.|

## Writing Opened Files
|Method|What It Does|
|---|---|
|.write(string)|This writes the string to the file.|
|.writelines(seq)|This writes the sequence to the file. No line endings are appended to each sequence item. It’s up to you to add the appropriate line ending(s).|

## \_\_file\_\_:
> Similar to \-\-name\-\-. When script is called, it wtill return path.

# [Exceptions](https://realpython.com/python-exceptions/)

We can use *raise* to throw an **Exception** if an condition occurs. 

```x = 10
if x > 5:
    raise Exception("Oops")
```

We can *assert* an exception when a specific condition is met.

```
import sys
assert ('linux' in sys.platform), "This code runs on Linux only."
```
## Try...except

The try...except block is used to handle exceptions. Anything wrong in try block will go stright to exception block and the codes in exception block will be triggered. This make the program conitnue to run without crash.
> Catching exception hides all errors so that you won't know what error you encounter when you use bare except clause. Therefore, you should alway refer the specific error excetpion you want to catch. e.g. ```try...except Assertion Error as error:...```

## Try...except...else ... finally
> If there is not exception needs to handle, then got to **else** block. The **finally** block will run no matter there is an exception or not.
