# Number Sum

# Assignment

## Complete the number_sum function. It should add up all the numbers from 1 to n.
- number_sum(5) -> 1+2+3+4+5 -> 15
- number_sum(3) -> 1+2+3 -> 6

## Solution
    def number_sum(n):
        total = 0
        for n in range(0, n + 1):
            total += n
        return total
