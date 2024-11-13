# Week 1

## 200. Number of Islands
Loop through array, once find a '1', use DFS to mark 4 direction to 0 and count + 1
## 204. Count Primes
Use non-prime boolean array to store true/false from 0 to n. Starting from 2, if it is false(definately true for 2), count ++, in the meantime, looping pivot j from 2 until i * j < n and makr rest of them in array as true
## 217. Contains Duplicate
Loop through array, use hashset to store. Once !set.add(n) => return true;
## 242. Valid Anagram
Use int array to store s.charAt(i) - 'a'
## 1. Two Sum
Use hashmap to store value - index pair
## 49. Group Anagrams
For each string, use char array to store frequency of each character and put {charArray.toString, string} to HashMap
## 347. Top K Frequent Elements

## 128. Longest Consecutive Sequence
## 15. 3Sum
