# Leetcode-1672.-Richest-Customer-Wealth

# Description
You are given an m x n integer grid accounts where accounts[i][j] is the amount of money the i​​​​​​​​​​​th​​​​ customer has in the j​​​​​​​​​​​th​​​​ bank. Return the wealth that the richest customer has.

A customer's wealth is the amount of money they have in all their bank accounts. The richest customer is the customer that has the maximum wealth.

# Solution
In the given scenario we have been given a matrix accounts[i][j] where i is the customer and j is the money.
We need to calculate and return the customer with the maximum wealth in his account.
 Example:
Input: accounts = [[1,5],[7,3],[3,5]]
Output: 10
[1,5] is first customer
[7,3] is second customer
[3,5] is the third customer
First customer's wealth =1+5 => 6
Second customer's wealth = 7+3 => 10
Third customer's wealth = 3+5 => 8

Maximum wealth = 10 

Algorithm:
1. Create a variable named max_wealth which returns the maximum wealth . Initialise it as 0.
2. Loop through accounts array .
3. Sum up each customer's wealth.
4. Calculate the maximum wealth by comparing th max_wealth variable with current wealth.
5. Return the maximum wealth.

# Time Complexity
Let m = No of customers
n = No of banks per customer

We are using a for loop which runs for m customers and sums up the wealth of each m customer , n times.

Total Time:
O(mxn)
