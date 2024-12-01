# ColorVolume_Comparator

A Python-based 3D visualization tool for comparing professional color spaces like ACES and Alexa Wide Gamut in XYZ coordinate space. This tool enables visual analysis of color gamut volumes, making it useful for colorists, cinematographers, and color scientists.

![colorvolume_comparator](https://github.com/user-attachments/assets/30fea06c-42e7-4bea-963a-7f98301784e7)

## Features

- 3D visualization of color space volumes
- Support for multiple color spaces including:
  - Alexa Wide Gamut
  - ACES
- Accurate color primary representations
- Interactive 3D viewing with rotation and zoom
- Proper color space transformations from xy chromaticity to XYZ
- Visual comparison of overlapping gamut volumes
- Clear primary point visualization
- Coordinate axis reference system

## Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

### Step 1: Clone the Repository

```bash
git clone https://github.com/yourusername/color-space-visualizer.git
cd color-space-visualizer
```

### Step 2: Create a Virtual Environment (Optional but Recommended)

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### Step 3: Install Required Packages

```bash
pip install -r requirements.txt
```

Or install packages individually:

```bash
pip install numpy matplotlib scipy
```

## Usage

Basic usage:

```python
python color_space_visualizer.py
```

This will display the 3D visualization comparing Alexa Wide Gamut and ACES color spaces.

### Interacting with the Visualization

- Rotate: Click and drag with the left mouse button
- Zoom: Use the mouse wheel
- Pan: Click and drag with the right mouse button
- Reset view: Home button in the matplotlib window

## Technical Details

### Color Space Primaries

#### Alexa Wide Gamut
- Red: (0.7347, 0.2653)
- Green: (0.1152, 0.8264)
- Blue: (0.1001, 0.1062)
- White Point: D65 (0.3127, 0.3290)

#### ACES
- Red: (0.7347, 0.2653)
- Green: (0.0000, 1.0000)
- Blue: (0.0001, -0.0770)
- White Point: D60 (0.32168, 0.33767)

### Implementation Details

The tool implements the following key components:
- Chromaticity to XYZ conversion
- RGB to XYZ transformation matrices
- Convex hull calculation for gamut boundary visualization
- 3D plotting using Matplotlib

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development Setup

1. Fork the repository
2. Create a new branch for your feature
3. Implement your feature or bug fix
4. Submit a pull request

## Future Improvements

- Additional color space support (P3, Rec.2020, etc.)
- Gamut volume calculation
- Color space intersection analysis
- Export capabilities for visualization data
- Custom color space definition support
- GUI interface for color space selection

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Color space primary data from professional color science documentation
- Matplotlib for 3D visualization capabilities
- Scientific Python community for numerical computation tools

## Contact

For questions and support, please open an issue on the GitHub repository.
