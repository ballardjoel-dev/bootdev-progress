# List Division

## Assignment

Complete the divide_list() function. It takes a list and a number as input, and should return a new list that contains all the elements of the original list after dividing them by the second input.

## Example

    divided_list = divide_list([6, 8, 10], 2)
    print(divided_list)
    # [3.0, 4.0, 5.0]

## Start

    def divide_list(nums, divisor):
        pass
        
## Solution

    def divide_list(nums, divisor):
        divided_list = []
        for num in nums:
            divided_list.append(num / divisor)
        return divided_list
    
## Run Cases

    run_cases = [
        ([6, 8, 10], 2, [3.0, 4.0, 5.0]),
        ([1, 2, 3, 4], 1, [1.0, 2.0, 3.0, 4.0]),
    ]
