# Lua pairs iterator unexpected behavior

This repository demonstrates a potential issue with Lua's `pairs` iterator when used with tables that are modified during iteration.  The problem arises when a function recursively iterates through nested tables, modifying them in the process.  This can result in elements being skipped or an infinite loop.

The `bug.lua` file contains code that showcases this issue.  The `bugSolution.lua` file offers a possible solution demonstrating safer iteration techniques.

## How to reproduce

1. Clone the repository.
2. Run `bug.lua` using a Lua interpreter (e.g., `lua bug.lua`).
3. Observe the unexpected output.