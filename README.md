
# NumPy Learning

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

A comprehensive repository dedicated to learning and mastering NumPy, the cornerstone library for numerical computing in Python. This resource is designed for both beginners and experienced users looking to deepen their understanding of NumPy's capabilities.

## Table of Contents

- [Introduction](#introduction)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
  - [Array Creation](#array-creation)
  - [Array Indexing and Slicing](#array-indexing-and-slicing)
  - [Element-wise Operations](#element-wise-operations)
  - [Broadcasting](#broadcasting)
- [Contributing](#contributing)
- [License](#license)

## Introduction

NumPy is an essential Python library for numerical computations, providing high-performance multi-dimensional array objects and tools for working with them. This repository aims to provide a structured learning path that covers fundamental concepts and advanced techniques. By working through the examples and exercises, you will gain the ability to:

- Efficiently manipulate numerical data.
- Perform complex mathematical operations on arrays.
- Leverage broadcasting for concise and efficient code.
- Utilize NumPy in various scientific and data analysis tasks.

This repository provides hands-on examples and detailed explanations to solidify your understanding of NumPy.

## Getting Started

Follow these instructions to set up your environment and start using NumPy.

### Prerequisites

- Python 3.7 or higher
- pip package installer (usually included with Python installations)

### Installation

1.  **Clone the repository:**

    bash
    python3 -m venv venv  # Create the virtual environment
    source venv/bin/activate   # Activate on Linux/macOS
    # venv\Scripts\activate  # Activate on Windows (use this if the above command doesn't work)
    This repository is organized to provide a step-by-step learning experience. Each directory focuses on specific NumPy concepts or functionalities.

> To run the examples, navigate to the respective directory and execute the Python scripts. For example:

bash
> cd array_creation
> python basic_arrays.py
> - `np.array()`: Creates an array from a list or tuple.
- `np.zeros()`: Creates an array filled with zeros.
- `np.ones()`: Creates an array filled with ones.
- `np.arange()`: Creates an array with a range of values.
- `np.linspace()`: Creates an array with evenly spaced values over a specified interval.

# Creating arrays from lists
arr1 = np.array([1, 2, 3, 4, 5])
print("Array from list:", arr1)  # Output: Array from list: [1 2 3 4 5]

# Creating an array of zeros
arr_zeros = np.zeros((3, 3))  # 3x3 array of zeros
print("Array of zeros:\n", arr_zeros)
# Output:
# Array of zeros:
#  [[0. 0. 0.]
#  [0. 0. 0.]
#  [0. 0. 0.]]

# Creating an array of ones
arr_ones = np.ones((2, 2))  # 2x2 array of ones
print("Array of ones:\n", arr_ones)
# Output:
# Array of ones:
#  [[1. 1.]
#  [1. 1.]]

# Creating an array with a range of values
arr_range = np.arange(0, 10, 2)  # Start, stop, step
print("Array with range:", arr_range)  # Output: Array with range: [0 2 4 6 8]



### Array Indexing and Slicing

Accessing and modifying array elements using indexing and slicing:

arr = np.array([0, 1, 2, 3, 4, 5, 6, 7, 8, 9])

# Accessing elements
print("First element:", arr[0])  # Output: First element: 0
print("Sixth element:", arr[5])  # Output: Sixth element: 5

# Slicing
print("Elements from index 2 to 4:", arr[2:5])  # Output: Elements from index 2 to 4: [2 3 4]
print("Elements from the beginning to index 2:", arr[:3])   # Output: Elements from the beginning to index 2: [0 1 2]
print("Elements from index 4 to the end:", arr[4:])   # Output: Elements from index 4 to the end: [4 5 6 7 8 9]

# Slicing with a step
print("Every other element:", arr[::2])  # Output: Every other element: [0 2 4 6 8]
arr1 = np.array([1, 2, 3])
arr2 = np.array([4, 5, 6])

# Element-wise addition
print("Element-wise addition:", arr1 + arr2)  # Output: Element-wise addition: [5 7 9]

# Element-wise subtraction
print("Element-wise subtraction:", arr2 - arr1)  # Output: Element-wise subtraction: [3 3 3]



### Broadcasting

Broadcasting allows NumPy to perform arithmetic operations on arrays with different shapes:

# Multiplying an array by a scalar
print("Multiplying by a scalar:", arr * scalar)  # Output: Multiplying by a scalar: [2 4 6]

# Broadcasting a 2D array with a 1D array
arr2d = np.array([[1, 2, 3], [4, 5, 6]])
arr1d = np.array([10, 20, 30])

> Add more examples to cover additional NumPy functionalities such as:
> - Reshaping arrays
> - Stacking arrays
> - Linear algebra operations
> - Random number generation
> - File I/O

## Contributing

Contributions are highly encouraged! To contribute to this project, please follow these guidelines:

1.  **Fork the repository.**
2.  **Create a new branch** for your feature or bug fix:

3.  **Implement your changes** and ensure your code adheres to the project's coding standards.
4.  **Write clear, concise commit messages.**
5.  **Test your changes** thoroughly.
6.  **Submit a pull request** to the main branch.

Please ensure your pull request includes:

- A clear description of the changes.
- Relevant code comments and documentation.
- Any necessary updates to the README.

Your contributions will help make this repository a valuable resource for learning NumPy!

## License

