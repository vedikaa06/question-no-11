# question-no-11
Solution to the question no 11 on leet code 

11. Container With Most Water
You are given an integer array height of length n. There are n vertical lines drawn such that the two endpoints of the ith line are (i, 0) and (i, height[i]).

Find two lines that together with the x-axis form a container, such that the container contains the most water.

Return the maximum amount of water a container can store.

Notice that you may not slant the container.

How it works
Two pointers:

Start with one pointer at the beginning (left) and one at the end (right).

Calculate area:

Area = width (right - left) × height (shorter line between height[left] and height[right]).

Update max area.

Move the pointer pointing to the shorter line, hoping to find a taller one and increase area.

Repeat until pointers meet.
