# Shuffle Sum

Read N, then N integers on the next line. Randomly shuffle the values once, then print their sum.

The sum does not change when the order changes, so the grader can still have one correct answer. Your program should actually perform the shuffle before summing.

1 ≤ N ≤ 10000. Integers: -10^9 to 10^9.

Library hints:
- Python: `import random`, then `random.shuffle(values)`.
- C: seed `rand()` once and implement Fisher-Yates: for `i` from `N - 1` down to `1`, choose `j = rand() % (i + 1)` and swap the two values.
- C++: include `<algorithm>` and `<random>`, create an `std::mt19937`, then call `std::shuffle(values.begin(), values.end(), rng)`.
- Java: create one `Random rng = new Random();` and use Fisher-Yates with `j = rng.nextInt(i + 1)`.

Use a 64-bit integer for the sum in C, C++, and Java.

Time limit: 2 seconds per test.

Example Input:
```text
5
4 1 7 2 6
```

Example Output:
```text
20
```
