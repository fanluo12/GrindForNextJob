## 3. Longest Substring Without Repeating Characters
Sliding window, looping through right pointer and use hashset to store characters. Once character in the set, remove left pointer(starts from 0) until not in set
## 7. Reverse Integer
Key point is testing overflow for case 1534236469. When reversing finishes, it becomes 964632435 which exceeds 2147483647, so When a number exceeds [-2^31 - 1, 2^31 - 1] in Java, it wraps around into the negative range starting from 
and this behavior is due to two's complement representation.
## 5. Longest Palindromic Substring
## 9. Palindrome Number
