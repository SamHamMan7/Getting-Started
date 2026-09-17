# Random Hunt

Read N, then N distinct integers on the next line. Remember the first value. Repeatedly choose a random element from the list until you choose that first value, then print it.

Create the random-number generator once, outside the loop.

1 ≤ N ≤ 1000. Integers: -10^9 to 10^9.

Library hints:
- Python: `import random`, then `random.choice(values)`.
- C: seed `rand()` once, then choose `values[rand() % n]`.
- C++: with an `std::mt19937 rng`, use `std::uniform_int_distribution<int> pick(0, n - 1)`.
- Java: with `Random rng = new Random();`, choose `values[rng.nextInt(n)]`.

Time limit: 2 seconds per test.

Example Input:
```text
5
8 3 9 2 7
```

Example Output:
```text
8
```
