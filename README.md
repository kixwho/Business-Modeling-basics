# Business Problem

Given a range of prices we could charge customers, and a range of costs to produce each unit of the product, how does profit change with price and cost?

# Solution

Construct a two-way sensitivity table using a Python nested loop. [Python solution.](https://github.com/kixwho/Business-Modeling-basics/blob/main/Sensitivity%20analysis.ipynb)  In Excel, the same analysis is done using a what-if analysis.

<img width="497" height="366" alt="image" src="https://github.com/user-attachments/assets/fbde63d8-5b8c-439c-9b79-5dc81282ebb7" />

<p>

**As the unit cost increases, the profit-maximizing price increases as some of the cost increase is passed on to customers.**

The Python logic used here represents a highly reusable computational pattern: loop through a pair of inputs, then calculate outputs. Compared to Excel, which uses different functions depending on the type of analysis, Python is tailor-made for automation. A few lines of readable code can be easily modified to guide a number of business objectives.

Another example is found in the Appendix.

<br>

## Appendix - City Distance Problem

### Problem

Given the latitude and longitude of selected cities, create a table that gives the distance between any two of the listed cities.

### Intuition

The key idea is simple: take every possible pair of cities, then perform the same calculation on each pair. This familiar Excel lookup problem is also perfect for a Python nested loop. Solution (partial view):

<p>

<img width="781" height="194" alt="image" src="https://github.com/user-attachments/assets/9d1b9179-0fc1-4931-b190-1bfa9d0a3be4" />

### Python Solution

1. Import and clean up the data table
2. Create an empty grid of the cities using the pandas DataFrame constructor
3. Fill in the values. A nested loop goes through every possible pair of cities, looks up their coordinates, calculates the distance, then places the result in the corresponding cell.

### Excel Solution

1. With raw data highlighted in green, I first created a grid of all the cities. The horizontal row was created using Transpose Paste
2. In cell H4, I used the formula <img width="909" height="28" alt="image" src="https://github.com/user-attachments/assets/94b2d979-f67d-420e-9e46-6e5b24921e5b" />
3. Copied the formula across the entire table (highlighted in blue)
