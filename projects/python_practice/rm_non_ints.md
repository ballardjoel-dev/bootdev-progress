# Remove Non-Integers

## Assignment

Complete the remove_nonints() function. It takes a list and returns a new list but with all the non-integer types removed.

## Example
    new_list = remove_nonints(["1", 1, "3", "400", 4, 500])
    print(new_list)
    # [1, 4, 500]

## Start
    def remove_nonints(nums):
        pass


## Solution

    def remove_nonints(nums):
        num_list = []
        for num in nums:
            if type(num) == int:
                num_list.append(num)
        return num_list

## Run Cases

        run_cases = [
            (["200", 300, 2, False, "otherstring", 6], [300, 2, 6]),
            ([True, 300, 2, False, "otherstring", 76, 86, "morestrings"], [300, 2, 76, 86]),
        ]
