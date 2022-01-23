# Competitive Programming

## Tips

These tips were largely provided by the Leetcode Patterns repo [1]:

- If input array is sorted, then:
  - Binary search
  - Two pointers
- If asked for all permutations/subsets, then:
  - Backtracking
- If given a linked list, then:
  - Two pointers
- If given a tree/graph, then:
  - DFS
  - BFS
- If recursion is disallowed, then:
  - Stack
- If requested to solve in-place, then:
  - Swap corresponding values
- If asked for minimum/maximum subarray/subset, then:
  - Dynamic programming
- If asked for top/least K items, then:
  - Heap
- If asked for common strings, then:
  - Map
  - Trie
- Else:
  - Map/set for O(1) time & O(n) space
  - Sort input for O(nlogn) time and O(1) space

## Modulo Operation

### Properties

- Modulo operation with divisor `n` yields a result in the range `[0, n-1]`.
- The modulo operation is distributive:
  - `((a + b) % c) == (((a % c) + (b % c)) % c)`
  - `((a * b) % c) == (((a % c) * (b % c)) % c)`

### Common Uses

- Check if a number is even (`x % 2 == 0`) or odd (`x % 2 != 0`).
- Wrap index around a container of size `n` (e.g., circular array/buffer).
- Traversal of a matrix:
  - Row-wise: `mat[idx / nrows][idx % ncols]`
  - Column-wise: `mat[idx % nrows][idx / ncols]`

## Bit Manipulation

### Two's Compliment

- Note the relation: `-x = ~x + 1`
  - This means that `x` and `-x` share the same right-most bit.

### Right-Most Bit

Note: There are not simple equivalent operations for the left-most bit.

- Isolate: `x & (-x)`
- Unset: `x & (x - 1)`

### XOR

- XOR of zero and bit results in that bit: `0 ^ x = x`
- XOR of one and bit toggles that bit: `1 ^ x = 1 - x`

## References

1. [seanprashad/leetcode-patterns](https://github.com/SeanPrashad/leetcode-patterns)
