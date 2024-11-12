# Week 1

## 200. Number of Islands
Loop through array, once find a '1', use DFS to mark 4 direction to 0 and count + 1

## 204. Count Primes
Use non-prime boolean array to store true/false from 0 to n. Starting from 2, if it is false(definately true for 2), count ++, in the meantime, looping pivot j from 2 until i * j < n and makr rest of them in array as true
