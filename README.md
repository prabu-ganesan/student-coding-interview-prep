# Introduction
![image](https://github.com/user-attachments/assets/9d57b043-8479-4b5c-957f-baebcac77309)

# Agenda
10 Introduction
 - What to expect in coding interviews?
 - How to approach a coding problem?
 - How to prepare coding interviews. 
20 first code
30 excercise
20 verbalize
20 talk about one of the exercise problems. 
Slinding Window if there is time. 
20 second code

# How to prepare for the coding interview
![image](https://github.com/user-attachments/assets/cd3f9e0f-1fa6-4a71-a772-3c25977bbeb7)


![image](https://github.com/user-attachments/assets/334f2af8-3ec3-4f86-891e-afff4b53f7da)


What to Study?
![image](https://github.com/user-attachments/assets/67923cbb-c7c7-4ee8-a825-ad40428ccf11)


## 1 Pattern: Sliding Window
#### Types
 - Sliding window with fixed window size.
 - Dynamic sliding Window. Cater-piller technique where left follows the right based on the criteria.

#### Questions
- Maximum Sum Subarray of Size K (easy)
- Smallest Subarray with a given sum (easy)
- Sliding Window Maximum
- Longest Substring with K Distinct Characters (medium)
- Fruits into Baskets (medium)
- No-repeat Substring (hard) *
- Longest Substring with Same Letters after Replacement (hard)
- Longest Subarray with Ones after Replacement (hard) *
- Problem Challenge 1 - Permutation in a String (hard) *
- Problem Challenge 2 - String Anagrams (hard)
- Problem Challenge 3 - Smallest Window containing Substring (hard) *
- Problem Challenge 4 - Words Concatenation (hard) 

## 2. Pattern: Two Pointers
- Move Zeroes https://leetcode.com/problems/move-zeroes/
- Pair with Target Sum (easy) https://leetcode.com/problems/two-sum/
- Remove Duplicates (easy) https://leetcode.com/problems/remove-duplicates-from-sorted-array/
- Squaring a Sorted Array (easy) https://leetcode.com/problems/squares-of-a-sorted-array/
- Triplet Sum to Zero (medium) https://leetcode.com/problems/3sum/
- Triplet Sum Close to Target (medium) https://leetcode.com/problems/3sum-closest/
- Triplets with Smaller Sum (medium) https://leetcode.com/problems/3sum-smaller/
- Subarrays with Product Less than a Target (medium) * https://leetcode.com/problems/subarray-product-less-than-k/
- Problem Challenge 1 - Quadruple Sum to Target (medium) *
- String Compression https://leetcode.com/problems/string-compression/
  
## 3. Pattern: Tree Depth First Search
Traversals
   - Inorder   (Left, Root, Right) - https://leetcode.com/problems/binary-tree-inorder-traversal/
   - PreOrder  (Root, Left, Right) - https://leetcode.com/problems/binary-tree-preorder-traversal/
   - PostOrder (Left, Right, Post) - https://leetcode.com/problems/binary-tree-postorder-traversal/
   
Questions   
- Binary Tree Path Sum (easy) - https://leetcode.com/problems/path-sum/
- All Paths for a Sum (medium) * - https://leetcode.com/problems/path-sum-ii/
- Sum of Path Numbers (medium) - https://leetcode.com/problems/sum-root-to-leaf-numbers/
- Path With Given Sequence (medium) *
- Count Paths for a Sum (medium)
- Problem Challenge 1 - Tree Diameter (medium) *
- Problem Challenge 2 - Path with Maximum Sum (hard) *

Pre-order Traversal
 - Create BST from sorted Array https://leetcode.com/problems/convert-sorted-array-to-binary-search-tree/
 Idea: In BST, Left subtree values would be less than root value. Right substree values would be greater than root. 
 So if we pick middle element for root, we can call the helper method for left portion and right portion to get left and right subtrees constructed recursively.

## 4. Pattern: Tree Breadth First Search
- Binary Tree Level Order Traversal (easy)
- Binary Tree Vertical Order Traversal https://leetcode.com/problems/binary-tree-vertical-order-traversal/
- Reverse Level Order Traversal (easy) * 
- Zigzag Traversal (medium)
- Level Averages in a Binary Tree (easy)
- Minimum Depth of a Binary Tree (easy) 
- Level Order Successor (easy)
- Connect Level Order Siblings (medium)
- Problem Challenge 1 - Connect All Level Order Siblings (medium)
- Problem Challenge 2 - Right View of a Binary Tree (easy) 

## 5. Pattern: Topological Sort (Graph)
### Purpose:

  Given n elements and there are pre-requisites for some or all elements. 
  Naturally, We would want to process the elements that have no prerequisites first. Then the next set of elements that becomes free and so on.
  This approach is called Topological Sorting and helps to find 1) if all of them can be processed or not 2) if yes then order of them.
  
### How it is implemented

  Given elements can be considered as nodes in Graph and a directed graph can be built using Map of Lists 
  and an array to track indegrees of each node(prereq).
  Then do the BFS for each set of nodes that currently have not prereqs.
  Map<Integer, List<Integer>> adjList = new ArrayList<>();
  Keys would be nodes. List would be nodes that depend on the key.
  int[] indegrees = new int[n];
  or if characters need to be returned, 
   Map<Character, Integer> indegrees = new HashMap<>();
  if there is a cycle then all of the nodes would be processed.
  
### Questions:

- Course Schedule https://leetcode.com/problems/course-schedule/
- Course Schedule II https://leetcode.com/problems/course-schedule-ii/
- Alien Dictionary (hard) https://leetcode.com/problems/alien-dictionary/
- Problem Challenge 1 - Reconstructing a Sequence (hard) *
- Problem Challenge 2 - Minimum Height Trees (hard) *

## 6. Pattern: Merge/Count Intervals
- Compare Intervals(Meeting Rooms) https://leetcode.com/problems/meeting-rooms/
- Merge Intervals (medium) - https://leetcode.com/problems/merge-intervals/
- Insert Interval (medium) * - https://leetcode.com/problems/insert-interval/
- Intervals Intersection (medium) - https://leetcode.com/problems/interval-list-intersections/
- Conflicting Appointments (medium) - https://leetcode.com/problems/non-overlapping-intervals/
- Problem Challenge 1 - Minimum Meeting Rooms (hard) * - https://leetcode.com/problems/meeting-rooms-ii/  (Priority Queue can be used to find overlap too).
- Problem Challenge 3 - Employee Free Time (hard) * - https://leetcode.com/problems/employee-free-time/
- Minimum Number of Taps to Open to Water a Garden - https://leetcode.com/problems/minimum-number-of-taps-to-open-to-water-a-garden/

## 7. Pattern: Fast & Slow pointers (Floyd's Cycle Detection Algorithm)

# Use
 - Find cycle in the linked list
 - Find mid point of a linked list.

## Cycle can be detected using Set for O(n) space complexity or using Floye's Algorithm for O(1) Space Complexity.

Questions
- LinkedList Cycle (Floy's Cycle Detection Algorithm) https://leetcode.com/problems/linked-list-cycle/
- Middle of the LinkedList (easy) https://leetcode.com/problems/middle-of-the-linked-list/
- Start of LinkedList Cycle (Floy's Cycle Detection Algorithm) * https://leetcode.com/problems/linked-list-cycle-ii/
- Happy Number (easy) * https://leetcode.com/problems/happy-number/ 
- Find the Duplicate Number https://leetcode.com/problems/find-the-duplicate-number/
- Problem Challenge 1 - Palindrome LinkedList (medium) *
- Problem Challenge 2 - Rearrange a LinkedList (medium)
- Problem Challenge 3 - Cycle in a Circular Array (hard) *

## 8. Pattern: In-place Reversal of a LinkedList/LinkedList
- Reverse a LinkedList (easy) 
- Reverse a Sub-list (medium) 
- Reverse every K-element Sub-list (medium) *
- Problem Challenge 1 - Reverse alternating K-element Sub-list (medium)
- Problem Challenge 2 - Rotate a LinkedList (medium)

https://leetcode.com/list/50sfo32d/

## 9.Pattern: Cyclic Sort
- Cyclic Sort (easy)
- Problem Challenge 1 - Find the Corrupt Pair (easy)
- Problem Challenge 2 - Find the Smallest Missing Positive Number (medium)
- Problem Challenge 3 - Find the First K Missing Positive Numbers (hard) *
- 
## 10. Pattern: Two Heaps
- Find the Median of a Number Stream (medium) 
- Sliding Window Median (hard) *
- Maximize Capital (hard) * 
- Problem Challenge 1 - Next Interval (hard) 

## 11. Pattern: Backtracking

 ### Backtracking is an algorithm that can provide all possible solutions for a problem.
``` 
 BACKTRACKING TEMPLATES:
 
 TEMPLATE: 1
 
 IF INPUT CONTAINS DUPLICATES BUT OUTPUT SHOULD NOT CONTAIN IT, THEN SORT THE INPUT ARRAY.
 
 BACKTRACK {
   RUN A LOOP
      PICK AN OPTION AND ADD TO TEMP LIST/STRING BUILDER
      ADD THE TEMP LIST/STRING BUILDER TO THE RESULT
      CALL BACKTRACKING METHOD FOR REST OF THE ELEMENTS
      REMOVE THE OPTION FROM TEMPLIST
 }
TEMPLATE: 2
BACKTRACK {
   IF BASE CASE CRITERIA MET(Ex, TEMPLIST LENGTH == StartIndex Passed in)
      ADD THE TEMP LIST/STRING BUILDER TO THE RESULT
   RUN A LOOP
      PICK AN OPTION AND ADD TO TEMP LIST/STRING BUILDER
      CALL BACKTRACKING METHOD FOR REST OF THE ELEMENTS
      REMOVE THE OPTION FROM TEMPLIST
 }
```
 Solution: Backtracking
 
 Some Examples:
 https://leetcode.com/problems/subsets/discuss/27281/A-general-approach-to-backtracking-questions-in-Java-(Subsets-Permutations-Combination-Sum-Palindrome-Partitioning)
 
 Questions:

- Subsets(aka, combinations) (easy) - https://leetcode.com/problems/subsets/
- Subsets With Duplicates (easy) * - https://leetcode.com/problems/subsets-ii/
- Permutations (medium) * - https://leetcode.com/problems/permutations/
- Permutations II - https://leetcode.com/problems/permutations-ii/
- String Permutations by changing case (medium)
- Balanced Parentheses (hard) *
- Unique Generalized Abbreviations (hard) * 
- Problem Challenge 1 - Evaluate Expression (hard) *
- Problem Challenge 2 - Structurally Unique Binary Search Trees (hard) *
- Problem Challenge 3 - Count of Structurally Unique Binary Search Trees (hard)

## 12. Pattern: Modified Binary Search
- Find First and Last Position of Element in Sorted Array - https://leetcode.com/problems/find-first-and-last-position-of-element-in-sorted-array/
- Order-agnostic Binary Search (easy)
- Ceiling of a Number (medium) *
- Next Letter (medium)
- Number Range (medium) *
- Search in a Sorted Infinite Array (medium) *
- Minimum Difference Element (medium)
- Bitonic Array Maximum (easy)
- Problem Challenge 1 - Search Bitonic Array (medium)
- Problem Challenge 2 - Search in Rotated Array (medium) * 
- Problem Challenge 3 - Rotation Count (medium) *

## 13. Kadene's Algorithm to find the maximum sum of subarray(it could be max sum of shortest or longest).

 https://leetcode.com/problems/maximum-subarray/
 
## 14. Pattern: Bitwise XOR
- Find the Missing Number (easy) https://leetcode.com/problems/missing-number/
- Single Number (easy)
- Two Single Numbers (medium) *
- Complement of Base 10 Number (medium)
- Problem Challenge 1

## 15. Pattern Top 'K' Elements
- Top 'K' Numbers (easy)
- Kth Smallest Number (easy)
- 'K' Closest Points to the Origin (easy)
- Connect Ropes (easy) *
- Top 'K' Frequent Numbers (medium)
- Frequency Sort (medium) *
- Kth Largest Number in a Stream (medium)
- 'K' Closest Numbers (medium)
- Maximum Distinct Elements (medium)
- Sum of Elements (medium) 
- Rearrange String (hard)
- Problem Challenge 1 - Rearrange String K Distance Apart (hard) 
- Problem Challenge 2 - Scheduling Tasks (hard) *
- Problem Challenge 3 - Frequency Stack (hard) 

## 15. Top-K Elements Design Question with Add, Reset, Sum of Top K elements. 
Use this technique for Design questions that involve add, reset/remove and topK functions to be implemented.
In This technique, topK function can be implemented at the complexity of O(K) using Map+TreeMap vs O(nlogn) complexity of using Priority Queue.
Idea: 
 - Use Map to store key and value.
 - Use TreeMap to store value and the number of keys for it.
 - Use Collections.reverseOrder() if maximum of K needed.
 - Get entryset from tree map with constant time.
 - Iterate over entryset for K elements to get the K elements.
 - Remember this, last two steps are what makes this approach to work in O(K) vs O(nlogn). Do not use treemap.get() in this approach as it would cost O(logn) for every call on tree map.

 - Design a leaderboard https://leetcode.com/problems/design-a-leaderboard/

## 16. Pattern: Stack
Stack can be used for 
 - DFS in trees and graphs
 - Store previous results
   ```
   Ex: https://leetcode.com/problems/basic-calculator/
   In this program. what makes it complex - The Associative Property when substraction needs to be done.
      - Numeric calculation needs to follow the PEMDAS rule. that is perenthesis, exponents, Multiplication or Division(Left to right) 
        then Addition or Substraction(Left to Right).
      - So if we enounter a open bracket, we need to evaluate the substring first and then evaluate with the left side of it. 
      - Stack can be used for it. but we can not evaluate right to left using stack in this case. that is because. A+(B+C) = C+B+A. 
        But A-(B-C) is NOT equal to C-B-A. Ex. 1-2+3 = 2. It is NOT 4. Because it should be evaluated from left to right.
        so can we evaluate as we iterate from left to right? Yes. this example would show it how. 
        The idea is 
           - A-(B+C) is equal to A+(-B)+(-C). So we can always just do addition by multiplying value with previous sign which can be 1 or -1 for + and -.
             1-(2+3) = 1+(-2)+(-3) = -4.
           - when we see open bracket, push previous result and sign to stack. 
             once substring is evaluated which we can take previous sign and result and simply add them to get the overall result.
           - Operators + or - can be represented as 1 and -1 respectively
             This has two advantages. 1. it can be stored in the stack like actual numbers. 2. 
             nums can be multiplied with them to get the value so that we can always to addition. Ex. 3-2 can be done as 3+(-2).
    ```
    
  - push to stack and process later when current element meets criteria. 
    Largest Rectangle in Histogram https://leetcode.com/problems/largest-rectangle-in-histogram/
    
   https://leetcode.com/list/504xdrcr/ 
    
## 17. Pattern: Re-Arrange/group elements to place N positions away the same elements.

Since the expected result is only a count for the below question, we do not have to re-arrange the elements but would focus more on mimicking and calcuation.

### What is the idea?
If we are able to fill all the idle slots between an element with maximum frequency, then all other elements can be filled N positions part.
Ex. Input: ["A","A","A","B","B","C","C"], N =2(Number of positions each element should be away from itself).
A contains maximum frequency of 3. So it can be arranged as A B C A B C.
So A is separated out with B and C's. also B and C's are separated out. in this case we do not need any extra idle time. we can return length of array.
If there is any idle spot that could not be filled, then result would be length+idlespots that could not be filled for A.
### Why do we check this only for an element with maximum frequency?
If element with maxium frequency can be separated out then all other elements can be. In above example, we see two groups. ABC followed by ABC. 
If there are any other elements, then we can just append in each group. Ex if we have two D's. it would be ABCD and ABCD and so on.
### what happens if we could not fill the A?
If we could not fill the A, we would introduce the groups still with idle space and that can be used to separate out other elements as mentioned below with groups.
that is why only the element with maximum frequency matters.

- Tasks Scheduling (medium) https://leetcode.com/problems/task-scheduler/

## 18. Pattern: TreeSet+SlidingWindow
Idea: Hour+Minutes(HH:MM) can be converted into just minutes(HH*60+MM) and stored in sorted form in TreeSet.
Then it would be easier to navigate through TreeSet by Converting into an ArrayList and do a sliding Window of K elements.

https://leetcode.com/problems/alert-using-same-key-card-three-or-more-times-in-a-one-hour-period/

## 19. Pattern: K-way merge
- Merge K Sorted Lists (medium) *
- Kth Smallest Number in M Sorted Lists (Medium) 
- Kth Smallest Number in a Sorted Matrix (Hard) *
- Smallest Number Range (Hard) *
- Problem Challenge 1 - K Pairs with Largest Sums (Hard) 

## 20. Pattern :(Dynamic Programming) 0/1 Knapsack 
 
 https://leetcode.com/discuss/general-discussion/458695/Dynamic-Programming-Patterns
 https://leetcode.com/explore/learn/card/dynamic-programming/
 https://leetcode.com/problems/min-cost-climbing-stairs/discuss/476388/4-ways-step-by-step-from-recursion-top-down-dp-bottom-up-dp-fine-tuning/854030
 

Idea:
```
Use 2D Matrix to track the match. if we mimic it in a table, we can see that left to right diagonal to represent the match vs mismatch.
  a b c d
a 1 0 0 0
b 0 1 0 0
c 0 0 1 0
d 0 0 0 1

dp would look like this. Note, there is an extra row and column so that we can look up diagonally top left box to get the previous value.
   
 0 0 0 0 0 
 0 1 0 0 0
 0 0 1 0 0
 0 0 0 1 0
 0 0 0 0 1

```
Question:
- Maximum Length of Repeated Subarray https://leetcode.com/problems/maximum-length-of-repeated-subarray/

Idea:

- 0/1 Knapsack (medium)
- Equal Subset Sum Partition (medium) *
- Subset Sum (medium)
- Minimum Subset Sum Difference (hard) *
- Problem Challenge 1 - Count of Subset Sum (hard) 
- Problem Challenge 2 - Target Sum (hard) 

## 20 HashMap Problems

https://leetcode.com/problems/online-election/

## 21. Reservoir Sampling Algorithm

## 22. Finding Valley and Peak
- Problem Challenge 3 - Minimum Window Sort (medium) * https://leetcode.com/problems/shortest-unsorted-continuous-subarray/

## 23  Side by Side String Comparison with O(N) Complexity and CONSTANT Space.
- Problem Challenge 2 - Comparing Strings containing Backspaces (medium) https://leetcode.com/problems/backspace-string-compare/

## 24 How to use original Array to track visited elements to avoid extra space.
Idea: The idea is to negative the value in the corresponding index. This works ONLY IF the elements are in 1 to N range and the array length is also N. 
- Find All Duplicates in an Array https://leetcode.com/problems/find-all-duplicates-in-an-array/

## 25 In-place Sorting of elements from 1 to n for an array of length of N.
This works only when the elements range is equal to array length. Time Complexity O(N) ignoring constants. Space Complexity: O(1).
- Find all Missing Numbers (easy) https://leetcode.com/problems/find-all-numbers-disappeared-in-an-array/

## 26 Splitting String+Re-combining word by word from end +HashTable
Subdomain Visit Count https://leetcode.com/problems/subdomain-visit-count/

## 27 X and Y Axis Based Movement tracking

Robot Return to Origin - https://leetcode.com/problems/robot-return-to-origin/
Robot Bounded In Circle https://leetcode.com/problems/robot-bounded-in-circle/ 

## 28 Prefix Sum Technique using HashMap

#### Where is it used?
You might want to use the prefix sum technique for the problems like "Find a number of continuous subarrays/submatrices/tree paths that sum to target".

#### What is prefix Sum?

Prefix sum is a sum of the current value with all previous elements starting from the beginning of the structure.

![image](https://user-images.githubusercontent.com/65518150/111923314-fb300600-8a74-11eb-9b2f-5487f74d211d.png)

Example: https://leetcode.com/problems/subarray-sum-equals-k/solution/
But Refer to the Solution of https://leetcode.com/problems/path-sum-iii/ for the above question for better explanation.

![image](https://user-images.githubusercontent.com/65518150/111923406-72659a00-8a75-11eb-92d2-27ac3d6f8a9d.png)

There could be two situations. 
 - In situation 1, the subarray with the target sum starts from the beginning of the array. That means that the current prefix sum is equal to the target sum, and we increase the counter by 1.


 - In situation 2, the subarray with the target sum starts somewhere in the middle. That means we should add to the counter the number of times we have seen the prefix sum curr_sum - target so far: count += h[curr_sum - target].

The logic is simple: the current prefix sum is curr_sum, and some elements before the prefix sum was curr_sum - target. All the elements in between sum up to curr_sum - (curr_sum - target) = target.
#### Why count += h[curr_sum - target] works?
Since values can be negative. the prefix some can ascend before it can get to the target. 
In this case, though we found a new subarray, that sub array can be combined with all other previously found subarrays to make more subarrays.
Example:
{1,-1,1,-1,1,-1), target = 0
{1,-1} and {1,-1} are individual subarrays. but they can be combined to create the third one. 

##### Questions
  https://leetcode.com/problems/path-sum-iii/
  https://leetcode.com/problems/subarray-sum-equals-k/solution/
  https://leetcode.com/problems/subarray-sums-divisible-by-k/
  https://leetcode.com/problems/continuous-subarray-sum/

## 29 Greedy Algorithm
https://leetcode.com/list/5ik01ftj/

## 30 Booyer-Moore's Algorithm to find Majority Element

Majority Element is one that appears > n/2 times in array.

Idea: Majority Element is the the element whose count can n't be offset by the count of other elements.
https://leetcode.com/problems/majority-element/

## 31 Miscellaneous
- Kth Smallest Number (hard) *
