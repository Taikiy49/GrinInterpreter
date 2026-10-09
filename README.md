<div align="center">
  <h1>GrinInterpreter</h1>
  <p><strong>Python interpreter for the Grin language with variables, arithmetic, input/output, and control flow.</strong></p>
  <p>
    <img alt="Python" src="https://img.shields.io/badge/Python-303840?style=flat-square" />
    <img alt="Interpreter" src="https://img.shields.io/badge/Interpreter-303840?style=flat-square" />
  </p>
  <p><a href="#overview">Overview</a> · <a href="#getting-started">Getting started</a> · <a href="#repository-map">Repository map</a></p>
</div>

---

## Overview

An interpreter for the small Grin programming language. Parsing produces instructions that execute against variable state, labels, and a subroutine return stack.

## What’s inside

- Assignment, numeric and string input, and printing.
- Arithmetic with type-specific checks.
- Conditional and unconditional jumps, subroutines, and returns.

## Getting started

Use Python 3 and provide the original course `grin` lexer/parser package on your Python path:

```sh
python grin_interpreter.py
```

Enter Grin source through standard input and terminate the source with a line containing `.`. The `grin` support package is not included in this repository; an unrelated package with the same name is not a substitute.

## Repository map

| Location | Purpose |
| --- | --- |
| [`grin_interpreter.py`](./grin_interpreter.py) | Entry point and top-level error handling |
| [`read.py`](./read.py) | Parse source into executable instructions |
| [`print_module.py`](./print_module.py) | Instruction execution |
| [`operations.py`](./operations.py) | Arithmetic |
| [`go_methods.py`](./go_methods.py) | Jumps and subroutine control |

## Project status

Course project. Requires the original language support package. Source-level error handling is included, but the repository does not contain an automated test suite.
