# Modulo Operation

## Properties

- The modulo operation is distributive:
  - `(a + b) % c` is equivalent to `((a % c) + (b % c)) % c`
  - `(a * b) % c` is equivalent to `((a % c) * (b % c)) % c`

## Misc

- The result of a module operation with divisor `n` must fall in the range
`[0, n-1]`.
  - We can use this property to wrap 0-based indicies for containers.
