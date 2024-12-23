## 1. Two Sum
Use hashmap to store value - index pair
## 3. Longest Substring Without Repeating Characters
Sliding window, looping through right pointer and use hashset to store characters. Once character in the set, remove left pointer(starts from 0) until not in set
## 5. Longest Palindromic Substring
## 7. Reverse Integer
Key point is testing overflow for case 1534236469. When reversing finishes, it becomes 964632435 which exceeds 2147483647, so When a number exceeds [-2^31 - 1, 2^31 - 1] in Java, it wraps around into the negative range starting from 
and this behavior is due to two's complement representation.
## 9. Palindrome Number
## 11. Container With Most Water
## 15. 3Sum
## 49. Group Anagrams
For each string, use char array to store frequency of each character and put {charArray.toString, string} to HashMap
## 128. Longest Consecutive Sequence
## 200. Number of Islands
Loop through array, once find a '1', use DFS to mark 4 direction to 0 and count + 1
## 204. Count Primes
Use non-prime boolean array to store true/false from 0 to n. Starting from 2, if it is false(definately true for 2), count ++, in the meantime, looping pivot j from 2 until i * j < n and makr rest of them in array as true
## 217. Contains Duplicate
Loop through array, use hashset to store. Once !set.add(n) => return true;
## 242. Valid Anagram
Use int array to store s.charAt(i) - 'a'
## 347. Top K Frequent Elements







