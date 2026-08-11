# Mirror World: Real-time Symmetry Drawing Tool

Mirror World is an interactive Python-based drawing tool designed for Google Colab that allows users to create symmetrical art in real-time. By leveraging `matplotlib` for rendering and `ipywidgets` for interactivity, the tool reflects user inputs across various axes of symmetry.

## Features

- **Multiple Symmetry Modes**: Choose between Horizontal, Vertical, and Quadrant symmetry.
- **Real-time Interaction**: Use sliders to control the pen position and see reflections instantly.
- **Mathematical Precision**: Uses NumPy to calculate reflected coordinates dynamically.
- **Visual Feedback**: A clean, coordinate-based canvas to visualize geometric patterns.

## Installation

To run this notebook, ensure you have the following dependencies installed:

```bash
pip install matplotlib numpy ipywidgets
```

## Usage

1. Open the notebook in Google Colab.
2. Run the initialization cells to load dependencies and the `MirrorCanvas` class.
3. Use the **Interactive Mirror World** section to experiment with different symmetry types and pen coordinates.

## How It Works

The core logic resides in the `MirrorCanvas` class, which automatically generates mirrored points whenever a new point is added based on the selected `symmetry_type`:

- **Horizontal**: $(x, y) \rightarrow (x, -y)$
- **Vertical**: $(x, y) \rightarrow (-x, y)$
- **Quadrant**: $(x, y) \rightarrow (-x, y), (x, -y), (-x, -y)$
