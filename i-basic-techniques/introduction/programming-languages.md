# Programming languages

At the moment, the most popular programming languages used in contests are C++, Python and Java. For example, in Google Code Jam 2017, among the best 3,000 participants, 79% used C++, 16% used Python and 8% used Java \[29\]. Some participants also used several languages.

Many people think that C++ is the best choice for a competitive programmer, and C++ is nearly always available in contest systems. The benefits of using C++ are that it is a very efficient language and its standard library contains a large collection of data structures and algorithms.

On the other hand, it is good to master several languages and understand their strengths. For example, if large integers are needed in the problem, Python can be a good choice, because it contains built-in operations for calculating with 3 large integers. Still, most problems in programming contests are set so that using a specific programming language is not an unfair advantage.

All example programs in this book are written in C++, and the standard library’s data structures and algorithms are often used. The programs follow the C++11 standard, which can be used in most contests nowadays. If you cannot program in C++ yet, now is a good time to start learning.

## C++ code template

A typical C++ code template for competitive programming looks like this:

```cpp
#include <bits/stdc++.h>

using namespace std;

int main() {
  // solution comes here
}
```

The `#include` line at the beginning of the code is a feature of the g++ compiler that allows us to include the entire standard library. Thus, it is not needed to separately include libraries such as `iostream`, `vector` and `algorithm`, but rather they are available automatically.

The `using` line declares that the classes and functions of the standard library can be used directly in the code. Without the `using` line we would have to write, for example, `std::cout`, but now it suffices to write `cout`. The code can be compiled using the following command:

The code can be compiled using the following command:

```bash
g++ -std=c++11 -O2 -Wall test.cpp -o test
```

This command produces a binary file test from the source code `test.cpp`. The compiler follows the C++11 standard \(`-std=c++11`\), optimizes the code \(`-O2`\) and shows warnings about possible errors \(`-Wall`\).

