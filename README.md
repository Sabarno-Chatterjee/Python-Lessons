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

          Syntax:

            while condition:
                statement(s)

          Statements in the code block under while are executed repeatedly as long as the condition evaluates to True. Generally, one of the statements under while makes some change to a variable that causes the condition to evaluate to False after a certain number of iterations.

        

        * for loops; 

            Syntax:

                for value in sequence:
                    statement(s)
          

          Similar to while loops, for loops also support the break and continue statements. break is used for breaking out of the loop and continue is used for skipping ahead to the next iteration.



# PASS STATEMENT:


    if statements cannot be empty, there must be at least one statement in every if and elif block. You can use the pass statement to do nothing and avoid getting an error.

    eg:

    if a_number % 2 == 0:
    elif a_number % 3 == 0:
    print('{} is divisible by 3 but not divisible by 2')

    This will give out an error, as the if block is empty.

    BUT:

    if a_number % 2 == 0:
    pass
    elif a_number % 3 == 0:
    print('{} is divisible by 3 but not divisible by 2'.format(a_number))

    Output:

    9 is divisible by 3 but not divisible by 2



# BREAK AND CONTINUE STATEMENTS:


    --> break:
        
         You can use the break statement within the loop's body to immediately stop the execution and   break out of the loop (even if the condition provided to while still holds true).

         e.g:

         i = 1
         result = 1

         while i <= 100:
            result *= i
            if i == 42:
                print('Magic number 42 reached! Stopping execution..')
                break
            i += 1
    
         print('i:', i)
         print('result:', result)


    --> continue:

        Sometimes you may not want to end the loop entirely, but simply skip the remaining statements in the loop and continue to the next loop. You can do this using the continue statement.

        e.g:

        i = 1
        result = 1

        while i < 20:
            i += 1
            if i % 2 == 0:
                print('Skipping {}'.format(i))
                continue
        print('Multiplying with {}'.format(i))
        result = result * i
        
        print('i:', i)
        print('result:', result)


# range:

    The range function is used to create a sequence of numbers that can be iterated over using a for loop. It can be used in 3 ways:

    range(n) - Creates a sequence of numbers from 0 to n-1
    range(a, b) - Creates a sequence of numbers from a to b-1
    range(a, b, step) - Creates a sequence of numbers from a to b-1 with increments of step


