# TinyGradEngine
A minimalistic gradient cmputaotion library implemented from scratch. This project is inspired by the idea of creating a lightweight, educational deep learning tool to understand the foundations of automatic differentiation and backpropagation.

## Features

- **Automatic Differentiation:** Perform efficient backpropagation for scalar values.
- **Educational:** Written in a clear and concise manner to help understand the basics of gradient computation.
- **Lightweight:** Minimal codebase to focus on core concepts.

## Project Structure

- **Code Cells:** Contains the core implementation of the TinyGradEngine library.
- **Markdown Cells:** Provides explanations and context for the code.
- **Examples:** Demonstrates the usage of the library for gradient computation and simple optimization tasks.

## Getting Started

### Prerequisites

- Python 3.7+
- Jupyter Notebook

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/TinyGradEngine.git
   cd MicroGrad
   ```

2. Install required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Open the Jupyter Notebook:

   ```bash
   jupyter notebook TinyGradEngine.ipynb
   ```

## Usage

1. Run the cells sequentially to load the library and execute examples.
2. Modify the examples or write your own code to experiment with the library.

## Examples

```python
from TinyGradEngine import Value

# Create variables
x = Value(2.0)
y = Value(-3.0)
z = Value(4.0)

# Perform operations
q = x * y + z
q.backward()

# Print gradients
print(f"Gradient of x: {x.grad}")
print(f"Gradient of y: {y.grad}")
print(f"Gradient of z: {z.grad}")
```
