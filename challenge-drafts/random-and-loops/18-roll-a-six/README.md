# Roll a Six

There is no input. Repeatedly generate a random integer from 1 through 6 until you generate 6. Print only the final `6`.

Create or seed your random-number generator once, before the loop. Do not recreate or reseed it on every roll.

Library hints:
- Python: `import random`, then `random.randint(1, 6)`.
- C: include `<stdlib.h>` and `<time.h>`, call `srand((unsigned)time(NULL));` once, then use `rand() % 6 + 1`.
- C++: include `<random>`, create `std::mt19937 rng(std::random_device{}());`, then use `std::uniform_int_distribution<int> die(1, 6);`.
- Java: `import java.util.Random;`, create `Random rng = new Random();`, then use `rng.nextInt(6) + 1`.

Time limit: 2 seconds per test.

Example Input:
```text
```

Example Output:
```text
6
```
