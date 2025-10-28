# C++ Basic Input/Output

**Day 1 of 6 Month DSA Challenge**  
**Date:** 28/10/2025

---

## Introduction
This document summarizes the basics of input and output in **C++**, an essential starting point before diving into Data Structures and Algorithms.
Understanding how to take input and print output is fundamental because every algorithm interacts with data through I/O.

---

## Including Libraries
C++ uses libraries to access functionality like input and output.
The library used for basic I/O is:

```cpp
#include <iostream>

```

`iostream` provides:

- `std::cout` → Output to screen
- `std::cin` → Input from keyboard

**Reference:**

https://en.cppreference.com/w/cpp/io

---

## Basic Program Structure

```cpp
#include <iostream>

int main() {
    // Your code here
    return 0;
}

```

The `main()` function is the entry point of every C++ program.

---

## Printing Output Using `cout`

```cpp
#include <iostream>

int main() {
    std::cout << "Hey, Striver!";
    return 0;
}

```

### Printing on a New Line

Use:

- `\n` (recommended — faster)
- `std::endl` (slower — flushes buffer)

```cpp
std::cout << "Hello\n";
std::cout << "World";

```

**Performance Note:**

`\n` is faster than `std::endl` because `std::endl` forces a buffer flush.

Reference: https://en.cppreference.com/w/cpp/io/manip/endl

---

## Using `using namespace std;`

To avoid writing `std::` repeatedly:

```cpp
#include <iostream>
using namespace std;

int main() {
    cout << "Hello World";
    return 0;
}

```

However, in professional large-scale code, it's avoided to prevent naming conflicts.

**Reference:**

https://isocpp.org/wiki/faq/coding-standards#using-namespace-std

---

## Taking User Input Using `cin`

```cpp
#include <iostream>
using namespace std;

int main() {
    int x;
    cin >> x;
    cout << "Value of x: " << x;
    return 0;
}

```

For multiple inputs:

```cpp
cin >> x >> y;

```

---

## `#include <bits/stdc++.h>` Shortcut (Optional)

This header includes most standard libraries, useful in CP/DSA, not recommended in production.

```cpp
#include <bits/stdc++.h>
using namespace std;

```

**Reference:**

https://stackoverflow.com/questions/31816095/what-is-bits-stdc-h-why-we-can-use-it

---

## ✅ Task Program: `printNumber`

```cpp
#include <iostream>
using namespace std;

void printNumber() {
    int n;
    cin >> n;       // input
    cout << n;      // output
}

int main() {
    printNumber();
    return 0;
}

```

---

## Summary

| Concept | Description |
| --- | --- |
| `iostream` | Enables basic I/O |
| `cout` | Prints output |
| `cin` | Accepts input |
| `\n` | Inserts newline efficiently |
| `std::endl` | Newline + flush (slower) |
| `using namespace std` | Avoids writing `std::` repeatedly |

---

## Progress

✅ Completed **C++ Basic I/O**

📆 **Day 1/180 of DSA Journey**

🚀 Next: Variables & Data Types