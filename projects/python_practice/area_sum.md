# Area Sum

## Assignment

Complete the area_sum() function. It accepts a list of rectangles, where each rectangle is a dictionary that has the following structure:

    {
      "height": 5,
      "width": 6
    }

It should calculate the area of each rectangle and return the sum of all the areas.

## Start

    def area_sum(rectangles):
        pass

## Solution

    def area_sum(rectangles):
        total_area = 0
        for rectangle in rectangles:
            total_area += rectangle["height"] * rectangle["width"]
        return total_area
