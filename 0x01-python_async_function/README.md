# 0x01. Python - Async

![Async Programming Meme](https://media.makeameme.org/created/python-programmers-python.jpg)

## Overview

This project focuses on asynchronous programming in Python using `asyncio`. You will learn how to write asynchronous code with `async` and `await`, manage concurrent coroutines, and create asynchronous tasks. This is an essential skill for building highly efficient, non-blocking Python applications, especially in back-end development.

---

## Learning Objectives

By the end of this project, you will be able to:

- Understand the `async` and `await` syntax.
- Execute an asynchronous program using `asyncio`.
- Run multiple coroutines concurrently.
- Create and manage `asyncio` tasks.
- Use the `random` module for simulating asynchronous events.

---

## Requirements

- **Environment**: Ubuntu 18.04 LTS
- **Python Version**: Python 3.7
- **Style Guide**: Pycodestyle (version 2.5.x)
- **Mandatory Files**:
  - `README.md`: Documentation for the project.
  - All Python modules must have proper documentation.
  - All functions and coroutines must have type annotations.
- **Execution**: All scripts must be executable.
- **Shebang**: The first line of all Python files must be `#!/usr/bin/env python3`.
- **File Length**: Will be tested using the `wc` command.
- **Documentation**: 
  - Modules, functions, and methods must have a meaningful, detailed docstring.
  - Use `python3 -c 'print(__import__("module_name").__doc__)'` to verify module documentation.
  - Use `python3 -c 'print(__import__("module_name").function_name.__doc__)'` to verify function documentation.

---

## Tasks

### Task 0: The Basics of Async
- **Objective**: Write a coroutine that waits for a random delay between 0 and 10 seconds and then returns the delay.
- **Prototype**: `async def wait_random(max_delay: int = 10) -> float:`
- **Usage**: Use the `random.uniform` function to generate the delay.

### Task 1: Run Multiple Coroutines
- **Objective**: Write a function that spawns multiple coroutines and returns their results in ascending order of completion.
- **Prototype**: `async def wait_n(n: int, max_delay: int) -> List[float]:`

### Task 2: Measure Execution Time
- **Objective**: Measure the total execution time of running multiple coroutines and compute the average time.
- **Prototype**: `def measure_time(n: int, max_delay: int) -> float`

### Task 3: Creating Tasks
- **Objective**: Write a function that returns an `asyncio.Task` for a coroutine.
- **Prototype**: `def task_wait_random(max_delay: int) -> asyncio.Task`

### Task 4: Concurrent Tasks
- **Objective**: Create a function that runs multiple asynchronous tasks concurrently.
- **Prototype**: `async def task_wait_n(n: int, max_delay: int) -> List[float]`

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/alx-interview.git
   cd alx-interview/0x01-python_async

