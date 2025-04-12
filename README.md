# ViewTree

**ViewTree** is a Python library designed to visualize binary trees using Graphviz. It provides functionality to render trees with proper spacing, alignment, and uniform node sizes, making it easy to debug and understand tree structures.

---

## Features

- **Binary Tree Visualization**: Render binary trees with proper alignment and uniform node sizes.
- **Distinguishable Children**: Clearly distinguishes left and right child nodes, with visual cues for `None` children.
- **Easy-to-Use API**: Simple functions to integrate tree visualization into your projects.
- **Graphviz Integration**: Leverages the powerful Graphviz library for high-quality rendering.

---

## Installation

You can install this package directly from GitHub using pip:

```bash
pip install git+https://github.com/isaamrat/tree_visualizer.git
```

For colab you can use the following pip command:

```bash
!pip install git+https://github.com/isaamrat/tree_visualizer.git
```

---

## Usage

Here is an example of how to use the library to visualize a binary tree:

```python
from viewtree import viewTree

class Node:
  def __init__(self, elem, left = None, right = None):
    self.elem = elem
    self.left = left
    self.right = right

# Example binary tree
root = Node(1,
                left=Node(2,
                             left = Node(4),
                             right = Node(5)),
                right=Node(3))

# Visualize the tree
viewTree(root)
```

After running the code, the binary tree will be rendered and saved as an image (`binary_tree.png`) in your working directory.
This will show:

![image](https://github.com/user-attachments/assets/ed6250bc-d3f5-44cc-b18f-a79120872b8e)


---

## API Reference

### `viewTree(root)`

- **Description**: Visualizes a binary tree and renders it as a PNG image.
- **Parameters**:
  - `root`: The root node of the binary tree.

### `visualize_tree(root)`

- **Description**: Generates a Graphviz `Digraph` object representing the binary tree.
- **Parameters**:
  - `root`: The root node of the binary tree.
- **Returns**: A `Digraph` object that can be rendered into various formats.

---

## Requirements

- Python 3.6 or higher
- `graphviz` (Python library)
- `ipython` (for displaying images in Jupyter Notebooks)

Install dependencies with:

```bash
pip install -r requirements.txt
```

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request on the [GitHub repository](https://github.com/your_username/viewtree).

---

## Acknowledgments

- [Graphviz](https://graphviz.org/) for providing the tools to create beautiful tree visualizations.
- The Python community for inspiring the creation of this library.

---

## Contact

For any questions or feedback, please contact [ext.md.khaliduzzaman@bracu.ac.bd].

