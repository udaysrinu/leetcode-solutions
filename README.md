# leetcode-solutions

C++ solutions to LeetCode problems, written while grinding DSA in college.

## What this is

2020 college-era practice work — not a polished study guide, not a curated
"top 150" list. Just the raw dump of my submissions as I worked through
problems and the daily LeetCoding Challenges (May–September 2020).

These solutions reflect my understanding *at the time of writing*. Some are
clean, some are brute-force first passes, some have leftover `cout` debug
lines. I'm leaving them as-is — rewriting old practice code defeats the
point of keeping it around.

## Contents

Roughly 430 `.cpp` files, organized in the laziest possible way: flat
directory, mostly named by LeetCode problem number.

Two naming patterns coexist:

- **`<problem-number>.cpp`** (e.g. `1.cpp`, `200.cpp`, `72.cpp`) — solution to
  the corresponding LeetCode problem. Suffixes like `(a)`, `(b)` are
  alternate attempts (different approach, optimization, or retry).
- **`leetcode-...-challenge-...-week-N-XXXX.cpp`** — daily challenge
  submissions from the 30-Day / monthly LeetCoding Challenges across
  May, June, July, August, September 2020.
- A few descriptively-named files (`Edit Distance.cpp`, `LCA of Binary tree.cpp`,
  `Clone a Linked List.cpp`, `Maximum width of tree.cpp`, etc.) — typically
  GeeksforGeeks-style problems or ones I saved before learning the LC number.

Topics covered span the usual interview-prep surface area: arrays, strings,
two pointers, sliding window, hashing, linked lists, stacks/queues, trees
(traversals, BST, LCA), graphs (DFS/BFS, islands), backtracking, greedy,
binary search, and DP (edit distance, knapsack-style, LIS, palindromes).

Difficulty mix is unlabeled here, but skews Easy/Medium with a handful of
Hard problems (e.g. `72`, `124`, `23`, `4*` ranges).

## How to use

There's no build system — each file is a standalone `class Solution { ... };`
meant to be pasted into the LeetCode editor. To browse:

- Know the problem number? Open `<num>.cpp`.
- Looking for a daily challenge? Search by month/week in the filename.
- Want to compile locally? Wrap the class in a `main()` with sample input;
  `g++ -std=c++17 file.cpp` will do it.

## What I'd do differently today

- **Organize by pattern, not by problem number** — folders like `dp/`,
  `graphs/`, `two-pointers/`, `trees/` would make this useful as a reference
  instead of an archive.
- **One README note per solution** — at minimum, time/space complexity and
  the key insight. Walking back into `200.cpp` cold today, I have to re-read
  it to remember why it works.
- **Tests** — even a tiny `assert`-based driver per file would catch the
  off-by-one regressions that LeetCode's online judge silently masked.
- **Drop the duplicates** — `342.cpp` / `342(a).cpp` / `342(b).cpp` should
  be one file with three commented approaches.
- **Stop committing `New Text Document.txt`.**

## License

No license file. Personal practice code; treat as reference only.
