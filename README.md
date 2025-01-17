# Chicken Animation Project 🐔

A delightful Python application that brings hand-drawn chicken sketches to life through simple animation. This project uses Pygame to create smooth animations from individual pencil drawings, making it perfect for artists and developers interested in traditional animation techniques.

## 🌟 Features

- Frame-by-frame animation support for pencil drawings
- Smooth transition between animation frames
- Interactive controls for animation playback
- Support for various image formats (PNG, JPG)
- Adjustable animation speed
- Simple and intuitive user interface

## 🛠️ Technical Requirements

- Python 3.8 or higher
- Pygame 2.5.2
- Pillow 10.2.0
- Compatible with Windows, macOS, and Linux

## 📋 Prerequisites

Before running the application, ensure you have Python installed on your system. You can download Python from [python.org](https://python.org).

## 🚀 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/chicken-animation.git
cd chicken-animation
```

2. Create and activate a virtual environment:
```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

3. Install required packages:
```bash
pip install -r requirements.txt
```

## 🎮 Controls

- **SPACE**: Pause/Resume animation
- **LEFT ARROW**: Decrease animation speed
- **RIGHT ARROW**: Increase animation speed
- **ESC**: Exit application

## 🎨 Adding Your Own Animations

1. Create your chicken drawings:
   - Draw each frame of your animation
   - Ensure consistent size and positioning
   - Use clean, high-contrast lines for best results

2. Prepare your images:
   - Save each frame as a PNG or JPG file
   - Name files sequentially (e.g., frame001.png, frame002.png)
   - Place all frames in the `assets/chicken_frames` directory

3. The animation will automatically load and play your frames in alphabetical order

## 📁 Project Structure

```
chicken_animation/
├── README.md           # Project documentation
├── requirements.txt    # Python dependencies
├── src/
│   ├── __init__.py
│   ├── main.py        # Main application entry point
│   └── chicken.py     # Animation logic
└── assets/
    └── chicken_frames/ # Directory for animation frames
```

## 🔧 Customization

You can modify various aspects of the animation:

1. Window Size:
   - Open `src/main.py`
   - Modify `WINDOW_SIZE = (800, 600)` to your preferred dimensions

2. Animation Speed:
   - Default speed can be adjusted in `src/chicken.py`
   - Modify `self.animation_speed = 0.1` in the `ChickenAnimation` class

3. Background Color:
   - Find `screen.fill((255, 255, 255))` in `main.py`
   - Change RGB values to your desired color

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🎬 Example Usage

```python
# Basic usage example
from src.chicken import ChickenAnimation
import pygame

pygame.init()
screen = pygame.display.set_mode((800, 600))
chicken = ChickenAnimation()

# Main loop
while running:
    chicken.update()
    chicken.draw(screen)
    pygame.display.flip()
```

## 🐛 Troubleshooting

Common issues and solutions:

1. **No frames loading:**
   - Check if your images are in the correct directory
   - Verify file extensions (.png or .jpg)
   - Ensure file permissions are correct

2. **Animation is too fast/slow:**
   - Use arrow keys to adjust speed
   - Modify base animation_speed in ChickenAnimation class

3. **Images not displaying correctly:**
   - Check image dimensions
   - Verify image format compatibility
   - Ensure images are not corrupted

## 📫 Contact

If you have any questions or suggestions, feel free to:
- Open an issue in this repository
- Submit a pull request
- Contact the maintainers

## 🙏 Acknowledgments

- Thanks to the Pygame community for the excellent gaming library
- Inspired by traditional animation techniques
- Special thanks to all contributors and users

Happy Animating! 🎨✨
