# Find Min
## Assignment

Write a function called find_min() that finds the smallest number in a list.

- find_min([1, 3, -1, 2]) -> -1
- find_min([18, 3, 7, 2]) -> 2

## Start
    def find_min(nums):
        pass


## Solution

    def find_min(nums):
        min = float("inf")
        for num in nums:
            if num < min:
                min = num
        return min
## Run Cases

        run_cases = [
            ([-4, -3, -2, -1, 0, 1, 2, 3, 4, 5, 6, 7], -4),
            ([4, 3, 2, 1, 18, 1, 2, 3, 4, 5, 6, 7], 1),
        ]
  
