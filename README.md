# system1

## Task

1. Fix the code so that all tests pass.

2. Add a document that explains what the code does.

3. Implement the `show()` method:

   - Implementation: implement it in `src/repo.cpp`:
     ```cpp
     void Repo::show(std::ostream &os) const;
     ```
   - Behavior: print the full internal structure in a readable way (at minimum: current head, branch heads, and the full commit chain(s)).
   - The CLI command `show` should print output (run `system1_cli` and type `show`).

## Constraints

- Use C++17.
- Do not remove or weaken tests.
- Keep public interfaces stable (do not rename public methods or change signatures unless truly necessary).
- You may refactor internally and add more tests.

## Build & Test

```bash
mkdir -p build
cd build
cmake ..
cmake --build .
ctest --output-on-failure
```
