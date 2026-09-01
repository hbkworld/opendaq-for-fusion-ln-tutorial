# Contributing

Thanks for considering a contribution to this tutorials repository!

## Adding a new tutorial

1. Create a new top-level folder, e.g. `tutorial_02` (or a short descriptive name).
2. Make it fully self-contained:
   - `README.md` with: overview, prerequisites, step-by-step instructions, and how to run it.
   - Its own dependency manifest (`requirements.txt`, `package.json`, `CMakeLists.txt`, etc.).
   - Any source code under a `src/` subfolder.
3. Do not depend on code from other tutorial folders — duplication is preferred over coupling.
4. Add a row for your tutorial to the table in the root [README.md](README.md).
5. Open a pull request.

## Style

- Keep instructions beginner-friendly and self-contained — assume the reader only reads that one tutorial's `README.md`.
- Prefer small, focused tutorials over broad ones covering many topics at once.
