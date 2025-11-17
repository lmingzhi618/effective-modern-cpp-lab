# Effective Modern C++ Lab
A hands-on learning repository for Effective Modern C++ by Scott Meyers.
This project implements code experiments, notes, and tests for each Item in the book, helping deepen understanding through practice rather than memorization.

---

## 🎯 Goals

* Write small, focused experiments for every Item in the book.
* Compare wrong vs. correct approaches emphasized by the author.
* Build intuition for modern C++ features:
  * Type deduction
  * auto and decltype
  * Move semantics & rvalue references
  * Smart pointers
  * Concurrency
  * And more
* Maintain concise notes for each Item (pitfalls, rules, insights).
* Validate behaviors with unit tests whenever possible.

📁 Repository Structure
```Bash
effective-modern-cpp-lab/
├── CMakeLists.txt
├── README.md
├── external/                 # External libraries (e.g., Catch2)
├── src/
│   ├── item01_deducing_types/
│   │   ├── note.md
│   │   ├── demo_*.cpp
│   │   └── test_*.cpp
│   ├── item02_auto/
│   ├── item03_moving_objects/
│   └── common/               # Utilities shared across Items
└── tests/
    └── main.cpp

```

## 🛠 Build & Run
### 1. Configure & build
```Bash
mkdir build && cd build
cmake ..
cmake --build . -j
```

### 2. Run all demos
```Bash
./emcpp_playground
```

### 3. Run tests
```Bash
ctest
# or
./emcpp_tests
```

### 🧪 Testing Framework
By default this repository uses Catch2 (v3).
It can be included via:
* external/catch2/
* or git submodule add https://github.com/catchorg/Catch2.git external/catch2

### 🚀 Learning Approach
For each Item:
1. Read the chapter
2. Reproduce the scenario from the book
3. Write:
  * an experiment demonstrating the idea
  * a note in your own words
  * optional tests to lock in your understanding
4. Commit with a clear message, e.g.:
```pgsql
Add Item01: Type deduction experiments
```
This creates a high-quality, practical notebook of modern C++ knowledge.

This creates a high-quality, practical notebook of modern C++ knowledge.

### 📚 Reference
Effective Modern C++ — Scott Meyers
C++ standard documentation: cppreference.com
