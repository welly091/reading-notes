# Class and objects

Classes are like a template to create objects. It has variables and functions that objects can inherent to use. 
We can create different objects that are of the same class.

\_\_init\_\_() function is a special function that is called when the class is being initiated. It's like a "constructor" in JavaScript.

# [Think Recursively](https://realpython.com/python-thinking-recursively/)

If the current problem does not represents a simple problem and can be divided into sub-problems with same strategy to solve them, use recursion.

List is not the only recursive data structure. Other examples include set, tree, dictionary, etc.

# [Pytest fixtures](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)
In some cases, you want to have some objects available to all of your tests. Those objects might contain data you want to share across tests, or they might involve the network or filesystem. We can use "pytest.fixtures" to approch this.

Define fixtures using "@pytest.fixture" decorator, along with the function you want other test functions to use. Then put this function as an "argument" in other test functions use.

Fixtures can acted like data. You also can decide how often a fixture is run.

