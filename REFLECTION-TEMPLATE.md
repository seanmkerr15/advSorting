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

1. Time complexity and reasoning:
2. Auxiliary space:
3. Stability and how my code preserves it:
4. Why Demo/Student comparison counts may differ:
5. Why a single short timing is insufficient:

## Demonstration checklist

- [ ] Student search and map
- [ ] Explain one merge comparison
- [ ] Show customization
