# 133
## 1. Two Sum
Use hashmap to store value - index pair
## 2. Add Two Numbers
## 3. Longest Substring Without Repeating Characters
Sliding window, looping through right pointer and use hashset to store characters. Once character in the set, remove left pointer(starts from 0) until not in set
## 5. Longest Palindromic Substring
## 7. Reverse Integer
Key point is testing overflow for case 1534236469. When reversing finishes, it becomes 964632435 which exceeds 2147483647, so When a number exceeds [-2^31 - 1, 2^31 - 1] in Java, it wraps around into the negative range starting from 
and this behavior is due to two's complement representation.
## 9. Palindrome Number
## 10. Regular Expression Matching
## 11. Container With Most Water
## 12. Integer to Roman
## 13. Roman to Integer
## 15. 3Sum
## 17. Letter Combinations of a Phone Number
## 19. Remove Nth Node From End of List
## 20. Valid Parentheses
## 21. Merge Two Sorted Lists
## 25. Reverse Nodes in k-Group
## 26. Remove Duplicates from Sorted Array
## 27. Remove Element
## 28. Find the Index of the First Occurrence in a String
Loop through string, for each index, use while loop to update needle index starting from 0, once finish updating, check if index ends at tail position of needle
## 33. Search in Rotated Sorted Array
## 35. Search Insert Position
## 36. Valid Sudoku
## 42. Trapping Rain Water
Two pointers starting from 0 and length - 1 index
## 45. Jump Game II
## 48. Rotate Image
## 49. Group Anagrams
For each string, use char array to store frequency of each character and put {charArray.toString, string} to HashMap
## 50. Pow(x, n)
Careful with overflow
## 53. Maximum Subarray
Use curSum to loop through array, once current sum is less than current value, raplace it
## 55. Jump Game
Update maxIndex variable when looping. Once maxIndex < current index, return false since it cannot reaches end
## 56. Merge Intervals
## 58. Length of Last Word
## 61. Rotate List
Make it to circular list
## 62. Unique Paths
## 63. Unique Paths II
## 64. Minimum Path Sum
## 66. Plus One
## 67. Add Binary
Like question two
## 69. Sqrt(x)
Binary search, when approaching middle pointer, careful with overflow, i.e. mid * mid may overflow
## 70. Climbing Stairs
Stair = 2 => [1, 1, 2]; Stair = 3 => [1, 1, 2, 3]; Initializing first two pointers with 1 and starting from 2, arr[i] = arr[i - 1] + arr[i - 2]
## 73. Set Matrix Zeroes
## 74. Search a 2D Matrix
## 76. Minimum Window Substring
## 77. Combinations
## 79. Word Search
## 80. Remove Duplicates from Sorted Array II
Use 2 pointers, left & right both starts from 0. From index 2 for left, as soon as nums[left - 2] != nums[right], make nums[left] = nums[right]
## 82. Remove Duplicates from Sorted List II
## 88. Merge Sorted Array
## 91. Decode Ways
## 92. Reverse Linked List II
## 97. Interleaving String
## 100. Same Tree
## 101. Symmetric Tree
## 102. Binary Tree Level Order Traversal
Use queue to store all the nodes, for each level, get queue size first, then loop through each level to get all the nodes' vals and add left/right sub-nodes to queue
## 104. Maximum Depth of Binary Tree
BFS update depth
## 112. Path Sum
## 120. Triangle
[4, 1, 8, 3, 0] -> []
## 121. Best Time to Buy and Sell Stock
Find minimum single price and in the same time find maximum profit
## 122. Best Time to Buy and Sell Stock II
Loop through prices array starting from index 1, as soon as current price greater than before, update profit value
## 125. Valid Palindrome
## 128. Longest Consecutive Sequence
## 130. Surrounded Regions
## 133. Clone Graph
## 134. Gas Station
## 136. Single Number
## 138. Copy List with Random Pointer
Deep copy use map
## 141. Linked List Cycle
one fast pointer and one slow pointer starting from head
## 149. Max Points on a Line
Loop through each point, for each point inner loop through points except for it. There are 3 cases, 1st is duplicates, this will need to be count also. 2nd is vertical, which dy dx is 0. 3rd will need to calculate slope and put into map as double
## 150. Evaluate Reverse Polish Notation
## 151. Reverse Words in a String
## 152. Maximum Product Subarray
maxProd & minProd
## 155. Min Stack
Use two stack, one regular stack and one min stack to trace minimum element
## 162. Find Peak Element
## 167. Two Sum II - Input Array Is Sorted
## 169. Majority Element
Declare majority number as nums[0] and count as 1, looping starts from index 1, once nums[i] == majority number, count ++, else count --, once count = 0, set current nums[i] as majority number
## 189. Rotate Array
nums = "----->-->"; k =3 result = "-->----->";
reverse "----->-->" we can get "<--<-----" reverse "<--" we can get "--><-----" reverse "<-----" we can get "-->----->"
## 190. Reverse Bits
## 191. Number of 1 Bits
## 198. House Robber
Use 1D dp array to update socre, dp[0] = nums[0], dp[1] = Math.max(nums[0], nums[1]), starting from index 2, dp[i] = max(dp[i] + nums[i - 2], dp[i - 1]). Note for case [2, 1, 1, 2], output is 4 for index 0 & 3. Not adjacent meaning dp[1] is max(nums[0], nums[1) instead of nums[1]
## 199. Binary Tree Right Side View
## 200. Number of Islands
Loop through array, once find a '1', use DFS to mark 4 direction to 0 and count + 1
## 202. Happy Number
Careful with cycle
## 204. Count Primes
Use non-prime boolean array to store true/false from 0 to n. Starting from 2, if it is false(definately true for 2), count ++, in the meantime, looping pivot j from 2 until i * j < n and makr rest of them in array as true
## 205. Isomorphic Strings
## 207. Course Schedule
## 208. Implement Trie (Prefix Tree)
## 209. Minimum Size Subarray Sum
## 210. Course Schedule II
## 211. Design Add and Search Words Data Structure
## 213. House Robber II
## 215. Kth Largest Element in an Array
## 217. Contains Duplicate
Loop through array, use hashset to store. Once !set.add(n) => return true;
## 221. Maximal Square
## 226. Invert Binary Tree
## 228. Summary Ranges
## 238. Product of Array Except Self
## 239. Sliding Window Maximum
## 242. Valid Anagram
Use int array to store s.charAt(i) - 'a'
## 261. Graph Valid Tree
## 271. Encode and Decode Strings
Original list of string: ["Hello", "World"], encoded => "5#Hello5#World"
## 274. H-Index
Sort and looping through new array, once current value >= length - current index, return length - current index
## 286. Walls and Gates
BFS update distance
## 287. Find the Duplicate Number
Fast and slow pointers
## 290. Word Pattern
## 300. Longest Increasing Subsequence
## 322. Coin Change
## 323. Number of Connected Components in an Undirected Graph
## 344. Reverse String
## 347. Top K Frequent Elements
Put all first k element in nums1 and nums2[0] into pq, then updating elements in nums2 to pq in while loop
## 373. Find K Pairs with Smallest Sums
## 380. Insert Delete GetRandom O(1)
## 383. Ransom Note
Use integer array to store frequency of all characters in magazine. Looping through ransomNote array, once a characte frequency is not 0, return false, else return true
## 392. Is Subsequence
## 417. Pacific Atlantic Water Flow
Use two array represents pacific and altantic. Use DFS to loop through and fill them
## 459. Repeated Substring Pattern
## 518. Coin Change II
## 567. Permutation in String
## 637. Average of Levels in Binary Tree
Using level order traversal, note that for each level, define a double variable to calculate sum for each level
## 647. Palindromic Substrings
Similar to question 5
## 684. Redundant Connection
## 695. Max Area of Island
## 704. Binary Search
if current length is 1, like [1], cannot use while (left < right)
## 739. Daily Temperatures
Use stack to push [value, index] pairs
## 746. Min Cost Climbing Stairs
## 787. Cheapest Flights Within K Stops
## 846. Hand of Straights
## 853. Car Fleet
Put current index and spped pair to an array and sort by ascending order of index. For each one, use stack to store expected time with double value. Once next value is <= stack.peek(), which means faster car will catch up previous at some point of time, don't do anything, else push to stack
## 875. Koko Eating Bananas
## 994. Rotting Oranges
## 1143. Longest Common Subsequence
2D dp array
## 1584. Min Cost to Connect All Points
Use pq to store [index, cost] pair and count to update current counted points








