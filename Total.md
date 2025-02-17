# 24 - 12/23/2024
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
## 26. Remove Duplicates from Sorted Array
## 27. Remove Element
## 35. Search Insert Position
## 49. Group Anagrams
For each string, use char array to store frequency of each character and put {charArray.toString, string} to HashMap
## 66. Plus One
## 70. Climbing Stairs
Stair = 2 => [1, 1, 2]; Stair = 3 => [1, 1, 2, 3]; Initializing first two pointers with 1 and starting from 2, arr[i] = arr[i - 1] + arr[i - 2]
## 80. Remove Duplicates from Sorted Array II
Use 2 pointers, left & right both starts from 0. From index 2 for left, as soon as nums[left - 2] != nums[right], make nums[left] = nums[right]
## 88. Merge Sorted Array
## 102. Binary Tree Level Order Traversal
Use queue to store all the nodes, for each level, get queue size first, then loop through each level to get all the nodes' vals and add left/right sub-nodes to queue
## 121. Best Time to Buy and Sell Stock
Find minimum single price and in the same time find maximum profit
## 125. Valid Palindrome
## 128. Longest Consecutive Sequence
## 162. Find Peak Element
## 169. Majority Element
Declare majority number as nums[0] and count as 1, looping starts from index 1, once nums[i] == majority number, count ++, else count --, once count = 0, set current nums[i] as majority number
## 200. Number of Islands
Loop through array, once find a '1', use DFS to mark 4 direction to 0 and count + 1
## 204. Count Primes
Use non-prime boolean array to store true/false from 0 to n. Starting from 2, if it is false(definately true for 2), count ++, in the meantime, looping pivot j from 2 until i * j < n and makr rest of them in array as true
## 215. Kth Largest Element in an Array
## 217. Contains Duplicate
Loop through array, use hashset to store. Once !set.add(n) => return true;
## 242. Valid Anagram
Use int array to store s.charAt(i) - 'a'
## 322. Coin Change
## 344. Reverse String
## 347. Top K Frequent Elements
## 373. Find K Pairs with Smallest Sums
Put all first k element in nums1 and nums2[0] into pq, then updating elements in nums2 to pq in while loop
## 383. Ransom Note
Use integer array to store frequency of all characters in magazine. Looping through ransomNote array, once a characte frequency is not 0, return false, else return true
## 459. Repeated Substring Pattern
## 637. Average of Levels in Binary Tree
Using level order traversal, note that for each level, define a double variable to calculate sum for each level







