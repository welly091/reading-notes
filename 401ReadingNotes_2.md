# [In Tests We Trust - TDD with Python](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)

## Unit tests and TDD?

TDD stand for Test-Driven Development- it's a strategy to think and write tests first then do develope later. 

Unit tests are some pieces of code to exercise the input, the output and the behaviour of code.

How to write a test name? The test file name should follow the same name of module name. 

e.g. module is *gender.py*, the test name should be *test_gender.py*

The AAA structure: 
- Arrange- organize the data needed to execute that piece of code
- Act- here you will execute the code being tested
- Assert- after executing the code, check if the result is the same as you were expecting

## The Cycle:
- We need to write a unit test and make it fail!
- Write the feature and make the test pass!
- Refactor the code- the first version doesn't need to be the beautiful one.

### The greatest advantage about TDD is to craft the software design first
### Your code will be more reliable: after a change you can run your tests and be in peace

# [If name equals main](https://www.geeksforgeeks.org/what-does-the-if-__name__-__main__-do/)
If the module is the main program, then code inside "\_\_main\_\_" should be running. 
If the file is imported from other module, then code inside "\_\_main\_\_" will not be execute.

# [What on Earth is Recursion](https://www.youtube.com/watch?v=Mv9NEXX1VHc)
Recursion is using the same function with calculated/updated input value over and over again until it reaches the end.

# [Python Strings](https://developers.google.com/edu/python/strings)
- Python strings are "immutable" 
- Double quotes or single quotes are ok.
- If you want to add a number with a string, you need to stringify the number first. e.g. str(4)
- There are some string built-in functions.

# [Python Lists](https://developers.google.com/edu/python/lists)
- list.append(elem) -- adds a single element to the end of the list. Common error: does not return the new list, just modifies the original.
- list.insert(index, elem) -- inserts the element at the given index, shifting elements to the right.
- list.extend(list2) adds the elements in list2 to the end of the list. Using + or += on a list is similar to using extend().
- list.index(elem) -- searches for the given element from the start of the list and returns its index. Throws a ValueError if the element does not appear (use "in" to check without a ValueError).
- list.remove(elem) -- searches for the first instance of the given element and removes it (throws ValueError if not present)
- list.sort() -- sorts the list in place (does not return it). (The sorted() function shown later is preferred.)
- list.reverse() -- reverses the list in place (does not return it)
- list.pop(index) -- removes and returns the element at the given index. Returns the rightmost element if index is omitted (roughly the opposite of append()).

# [Python Modules and Packages](https://realpython.com/python-modules-packages/)
- Modular programming refers to the process of breaking a large, unwieldy programming task into separate, smaller, more manageable subtasks or **modules**.
- Modules have several advatanges: simplicity, maintainability, reusability, scoping(avoid collisions between identifiers in different areas of a program).
- **from <module_name> import <names(s)> as <alt_name>**

- The built-in function dir() returns a list of defined names in a namespace.

- Packages organize modules and avoid collisions between module names.
- Packages allow for a hierarchical structuring of the module namespace using dot notation.
- If a file named **\_\_init\_\_.py**, it is invoked when the package or a module in the package is imported. This can be used for execution of package initialization code.

# [PyTest Tutorial](https://www.guru99.com/pytest-tutorial.html)
- PyTest is a testing framework that allows users to write test codes using Python programming language.
- **assert** is the result you want to compare with the function.
![assert](https://i.imgur.com/sfYXk3a.jpg)
- py.test -k method1 -v
  - -k <expression> is used to represent the substring to match
  - -v increases the verbosity
- Pytest allows us to set various attributes for the test methods using pytest markers, **@pytest.mark.<name>**. To use markers in the test file, we need to import pytest on the test files.
  e.g. ![pytest.mark](https://i.imgur.com/S9bc9Tp.jpg)
