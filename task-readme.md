  * [General information](#general)
  * [Run verdicts] (#verdicts)
  * [Languages](#languages)
    * [NodeJS](#nodejs)
    * [C++](#cpp)
    * [Python](#python)
    * [Java](#java)
    * [C#](#csharp)
    * [Ruby](#ruby)
    * [PHP](#php)
    * [Perl](#perl)

- - -

### <a name="general"></a>General Information

For solving **Codefights** challenges, you should implement a function in your preferred language. When submitted, your function is wrapped in a class/closure, so some declarations may result in a <b>Syntax (Compilation) Error</b>. Keep in mind the following:

1. Your code should declare a function/method with exactly the same name that is specified in the challenge. Changing its name will result in a syntax error. 
1. You can log any data in the console for debug purposes (e.g. _console.log_ in _JS_, _std::cout_ in _C++_).
1. If value of some input/output argument is string that contains double quote characters (`"`) it will be shown in the output with additional `\` symbol. E.g. `inputString` = `hello"world"hello`, it will be displayed in the console as `"hello\"world\"hello"`. 

### <a name="verdicts"></a>Verdicts
After submitting your code for testing, the following verdicts are possible: 

1. **Compilation/syntax error** - this means you most probably have some syntax errors in your source code. More detailed information will be given along with the verdict to help you identify the issue.
1. **Compilation time exceeded** - This verdict happens rarely and mostly for C++ or Java. This means that your code is either too long, or you overused templates, which results in very slow compilation of your code.
1. **Execution limit exceeded** - This means that your code didn't finish executing within the given time limit. It either got hung up on one of the test cases, or it just works very slowly. It's likely that your solution is either not optimally efficient, or you have a bug in the code.
1. **Output limit exceeded** - This verdict happens rarely. It means that either your function return value size is too big (e.g. you returned a very big array or matrix), or that you overused console outputs and essentially spammed it with lot of data. One possible cause of such an issue is that you have a console output inside the infinite loop.
1. **Wrong answer** - This verdict means that your code was compiled and ran successfully, but it returned an incorrect output for one or more test cases. More detailed information will be provided to help you diagnose the issue.
1. **All tests passed** - This means that your code works correctly and passed all the tests within the given time limit.

### <a name="languages"></a>Languages

We support a variety of compilers and languages. You can solve each task in your preferred language by clicking on the language switcher icon in the upper right corner of the IDE. In the next sections you will find detailed information on each available language and compiler.

#### <a name="nodejs"></a>NodeJS

We support _NodeJs v5.3.0_ compiler with almost all _ES2015_ features.
Some best practices for _Nodejs_. 

1. Please use `console.log()` to print any data for debugging purposes.
1. In order to declare variables with `let` keyword, add `use strict` at the beginning of the function. 
1. Use arrow functions `() => {}` and other _ES2015_ features to write concise and clear code.

#### <a name="cpp"></a>C++

We support _g++ 5.0_ with _C++14_ features enabled. Feel free to use `unordered_map, regex, range for, auto ...` features from _C++11_ and _14_ standards.
The following libraries are automatically included:
```
#include <iostream>
#include <vector>
#include <cstdarg>
#include <string>
#include <cstdio>
#include <cctype>
#include <cmath>
#include <queue>
#include <map>
#include <set>
#include <algorithm>
#include <climits>
#include <sstream>
#include <numeric>
#include <iterator>
#include <iomanip>
#include <utility>
#include <stack>
#include <functional>
#include <deque>
#include <complex>
#include <bitset>
#include <list>
#include <array>
#include <regex>
#include <unordered_set>
#include <unordered_map>
```

Some best practices for C++.

1. When declaring global variables in _C++_, initializing them during declaration will result in a syntax error. Instead, perform an initialization in the function/method. 
1. Static variables are disabled in _C++_, so using them will lead to unexpected results.
1. Add `using namespace std;` at the beginning of the function in order to use _std_ features without `std::` prefix.
1. Please use `std::cout` to print any data for debugging purposes.
1. Use C++11 and 14 features, e.g. `for (x: vec) {...} `, lambda functions  `[](int a, int b) -> bool {...}`.

#### <a name="python"></a>Python
The Python version used on the site is **2.7**. 

1. For further information about the differences between python3 and python2, consult [The Python Language Wiki](https://wiki.python.org/moin/Python2orPython3).
1. If python3 is your preferred version, [you might want to try out the 3to2 tool](https://wiki.python.org/moin/3to2).
1. Please use `print ...` to print any data for debugging purposes.

The following libraries are automatically imported:
```
import math
import string
import re
import random
```

#### <a name="java"></a>Java
The compiler used on the site is _Java7 1.7.0_. 

1. Please use `System.out.println(...)` to print any data for debugging purposes.
1. When declaring global variables in _Java_, initializing them during declaration will result in a syntax error. Instead, perform an initialization in the function/method.

Following libraries are automatically included: 
```
import java.io.*;
import java.util.*;
import java.math.*;
import java.util.regex.*;
import java.text.*;
```

#### <a name="csharp"></a>**C#**
The compiler used on the site is _Mono C# version 3.2.8.0_. Please use `Console.Write(...)` to print any data for debugging purposes.
The following libraries are included:
```
using System;
using System.IO;
using System.CodeDom.Compiler;
using System.Collections;
using System.Collections.Generic;
using System.ComponentModel;
using System.Diagnostics.CodeAnalysis;
using System.Globalization;
using System.Reflection;
using System.Runtime.Serialization;
using System.Text;
using SimpleJson.Reflection;
using System.Text.RegularExpressions;
using System.Linq;
```

#### <a name="ruby"></a>Ruby
The compiler used on the site is _Ruby 1.9.3_. Please use `puts ...` to print any data for debugging purposes.
The following libraries are automatically included:
```
require 'json'
require 'stringio'
```

#### <a name="php"></a>PHP
The compiler version used on the site is _PHP 5.6.4_. Please use `echo ...` to print any data for debugging purposes.

#### <a name="perl"></a>Perl
The compiler version used on the site is _Perl 5.20.2_. Please use `print ...` to print any data for debugging purposes.
The following libraries are automatically included:
```
use warnings;
use JSON;
```
