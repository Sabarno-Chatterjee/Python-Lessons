# Python-Lessons


LISTS:

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


