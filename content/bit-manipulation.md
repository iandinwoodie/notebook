# Bit Manipulation

## Two's Compliment

- Note the relation: `-x = ~x + 1`
  - This means that `x` and `-x` share the same right-most bit.

## Right-Most Bit

Note: There are not simple equivalent operations for the left-most bit.

- Isolate: `x & (-x)`
- Unset: `x & (x - 1)`

## XOR

- XOR of zero and bit results in that bit: `0 ^ x = x`
- XOR of one and bit toggles that bit: `1 ^ x = 1 - x`
