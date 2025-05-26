# Join Strings

## Assignment

Complete the join_strings() function. It takes a list of strings and returns a new single string. The new string is the concatenation of all the input strings from the list end-to-end, in order, with a comma between them.

## Example

    string_list = ["Annie", "Reiner", "Bertholdt"]
    joined_string = join_strings(string_list)
    print(joined_string)
    # "Annie,Reiner,Bertholdt"

    string_list = ["Eren", "Mikasa", "Armin"]
    joined_string = join_strings(string_list)
    print(joined_string)
    # "Eren,Mikasa,Armin"

## Start

    def join_strings(strings):
        pass

## Solution

    def join_strings(strings):
        joined_string = ""
        for string in strings:
            joined_string += string + ","
        return joined_string[:-1]

## Run Cases

    run_cases = [
        (["hello", "world"], "hello,world"),
        (["this", "list", "is", "so", "important"], "this,list,is,so,important"),
    ]
