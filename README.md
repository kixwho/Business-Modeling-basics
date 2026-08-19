## Problem

Given the latitude and longitude of selected cities, create a table that gives the distance between any two of the listed cities.

## Intuition

The key idea is simple: take **every possible pair** of cities, then perform the same calculation on each pair.

## Python Solution

1. Import and clean up the data table
2. Create an empty grid of the cities using the pandas DataFrame constructor
3. Fill in the values. A nested loop goes through every possible pair of cities, looks up their coordinates, calculates the distance, then places the result in the corresponding cell.

**Main advantage: Automation**. Instead of manually building and filling the grid, the entire process is handled by a few lines of readable code.

## Excel Solution

1. With raw data highlighted in green, I first created a grid of all the cities. The horizontal row was created using Transpose Paste
2. In cell H4, I used the formula <img width="909" height="28" alt="image" src="https://github.com/user-attachments/assets/94b2d979-f67d-420e-9e46-6e5b24921e5b" />
3. Copied the formula across the entire table (highlighted in blue)
