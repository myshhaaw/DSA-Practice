# Problem

Platform:striver
Difficulty: easy
Pattern:max , min , largest , smallest
Topic: Arrays
Date Solved: 7/07/26


---

## Problem Link
strivers a2z sheet first question 

## My First Thought
My First Thought
We are given an array arr and we need to find the largest element.
so we will begin sorting the elements
and the last elements of the sorted array will be the answer 
BUT 
doing all this unnecesarry work for one single element is not okay and it might take upto nlogn time complexity 
so i will



## Brute Force

Time Complexity: O(nlogn)

Space Complexity:O(n)

Why O(nlogn)?
considering merge or quick sort even 
Why O(n) space?
The output array has size 2n, which grows linearly with input size.

---

## Optimal Solution

Time Complexity:o(n)

Space Complexity:O(n)

---

## Code (C++)

Class Solution {
    public:
    int largest (vector<int>&arr){
        int largest = arr[0];
        for(int i=1;i<arr.size;i++){
            if(arr[i]>largest){
            largest = arr[i];
        }
        }
    }
    return largest;
}

---

## Dry Run
arr=[1,5,6,3,8]
int largest = 1 

i=1-->
is 5>1 ? yes--> int largest =5
i=2 -->
is 6>5 ? yes --> int largest =6
i=3
is 3>6 ? no --> int largest =6
i=4
is 8>6 yes --> int largest = 8 


## Edge Cases

---

## Mistakes I Made

---

## Pattern Recognition

How will I recognize this pattern next time?

whenever you see words like 
## Revision Notes

---

## Revisit

- [ ] 1 day
- [ ] 1 week
- [ ] 1 month
