# Python-Lessons

PYTHON DATA TYPES:

1. PRIMITIVE TYPES:

    i.e. Built in data types.

        integer, boolean, string, float,etc.

2. CONTAINERS:



        -->LISTS:

            # SLICING:


                Slicing
                You can also pull a segment of a list (for instance, the first three entries or the last two entries). This is called slicing. For instance:

                to pull the first x entries, you use [:x], and
                to pull the last y entries, you use [-y:].
                to pull entries from a specific startign point, till 2nd element. [0:3]

            # Removing items
                
                Remove an item from a list with .remove(), and put the item you would like to remove in parentheses.

            # Adding items

                Add an item to a list with .append(), and put the item you would like to add in parentheses.

            # You can also get the minimum with min(list_name) and the maximum with max(list_name).
            # To add every item in the list, use sum().
            # Sorted: sorted returns a sorted version of a list;
                    sorted(planets)



            List methods: A function attached to an object is called a method.

                1. list.append modifies a list by adding an item to the end.
                2. list.pop removes and returns the last element of a list.
                3. list.index() Where does an element fall in the order of the list? We can get its index using the  list.index method.


        -->DICTIONARY:

            A dictionary is an unordered collection of items. Each item stored in a dictionary has a key and value. You can use a key to retrieve the corresponding value from the dictionary. Dictionaries have the type dict.

            Dictionaries are often used to store many pieces of information e.g. details about a person, in a single variable. Dictionaries are created by enclosing key-value pairs within braces or curly brackets { and }.



        -->TUPLES:

            Tuples are almost exactly the same as lists. They differ in just two ways.
                1. The syntax for creating them uses parentheses instead of square brackets;
                    t = (1, 2, 3)
                2: They cannot be modified (they are immutable).





OPERATORS:


        # ABS:

            Returns the absolute value of an argument:
            print(abs(32))
            print(abs(-32))

            Will print:

            32
            32

        
* help()

    The help() function is possibly the most important Python function you can learn. If you can remember how to use help(), you hold the key to understanding most other functions.

    eg:

    help(round)


* docstrings


    def function_name(parameters):

    """ The docstring is a triple-quoted string (which may span multiple lines) that comes immediately after the header of a function. When we call help() on a function, it shows the docstring.
    """



* Higher-order functions

    Functions that operate on other functions are called "higher-order functions." 

    def mod_5(x):
    """Return the remainder of x after dividing by 5"""
    return x % 5

    print(
    'Which number is biggest?',
    max(100, 51, 14),
    'Which number is the biggest modulo 5?',
    max(100, 51, 14, key=mod_5),
    sep='\n',
    )


    Sol.

    Which number is biggest?
    100
    Which number is the biggest modulo 5?
    14



# Python Operators:


    1. Logical operators    :    and, or, not.
    2. Conditional operators:    >,<,=,etc.
    3. Arithmetic operators :    +, *, /, etc.


# PYTHON BRANCHING & LOOPS:

    -->CONDITIONAL STATEMENTS:

        if, elif and else statements.

        * CONDITIONAL EXPRESSION (ternary operator):

            Using this we can write a multi line if, else statement in a single line.

            Syntax:

            x = true_value if condition else false_value

            e.g:

            number = 'even' if a_number % 2 == 0 else 'odd'


    
    -->ITERATION (LOOPS):

        * while loops;

        

        * for loops; 



