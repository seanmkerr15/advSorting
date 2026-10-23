# Caffeine Quest reflection

Name: Sean Kerr

## Five questions before coding

1. **Purpose:** The purpose of the merge sort is to compare the distances of Starbucks locations to find the one closest to the stated latitude and logitude.
2. **Inputs and outputs:**  items is a list that needs to be sorted. Start and end are where the array begins and ends so the sort could work on that area. The list items is changed because the list is being sorted. A list of how many comparisons is returned.
3. **Constraints:** Both halves are already sorted. You can not use .sort methods.
4. **Edge cases:** When one half runs out then the half that didn't ran out get's put into the rest of the array. When keys are equal the program just chooses one and puts it in first, doesn't matter.
5. **Test oracle:** We can test using the demo mode in order to see if the merge sort is correct.

## Explore Demo mode

Starting latitude/longitude:

| Filter | Rank | Store ID / name | Distance in miles |
|---|---:|---|---:|
| All stores | 1 | | |
| All stores | 2 | | |
| All stores | 3 | | |
| Drive-through only | 1 | | |
| Drive-through only | 2 | | |
| Drive-through only | 3 | | |

**What changed, and why would alphabetical order not answer this search?**
_We stopped comparing the strings and starting to compare values in order to sort it by distance. Alphabetical order would not answer this search because it would only sort them by the letters of their name and would never give us the one closest._

## Hand trace: merge [2, 7] and [3, 5]

| Step | Compared values (if any) | Item copied | Buffer so far |
|---|---|---|---|
| 1 | | | |

## Validation

Final SortCheck output or evidence filename:

Additional test: input / expected output / actual output / reason:

Student-mode first three results for the two original searches:

How do they compare with Demo mode? Student map evidence filename:

## Investigate one feature (150-250 words)

Topic and class/method:

Short relevant code excerpt:

Explanation and concrete example:

Source consulted (title and URL or course reference):

## Customization

Feature:

Files changed and explanation:

New-feature test and result:

Default-behavior regression check:

## Algorithm explanation

1. Time complexity and reasoning: The time complexity of the algorithm is O(nlogn) this is because mergeSort is split up in two ways.
   The first step is separating elements the arrays into their individual arrays and that takes O(logn) time. Then when it comes to sorting and merging the elements back together in an array that takes O(n) time. When you combine them you get O(n*logn).
3. Auxiliary space: It's auxiliary space is O(n) this is because that for each element in the array a new array including one element is created. Therefore the computer has to store these elements somewhere in order to sort and merge them back so it must do for for each element in the array.
4. Stability and how my code preserves it: Stability is ensuring that two elements of equal value will be put into the array in the order they appeared. The code preserves this because the left-most array goes first and so the elements of equal value will be sorted into the order they appeared because the element that appeared first would be in the left-most array.
5. Why Demo/Student comparison counts may differ: The demo version used a sorting algorithm that did not have to rely on ram as much as the student sorting algorithm did. The merge sort may have been slower because it would have required more ram to complete it faster.
6. Why a single short timing is insufficient: The speed of a recursive algorithm depends on the ram. It cannot be determined based off o f a single short-timing because the timing will be inconsistent across multiple devices based on the level of ram available to the algorithm.

## Demonstration checklist

- [ ] Student search and map
- [ ] Explain one merge comparison
- [ ] Show customization
