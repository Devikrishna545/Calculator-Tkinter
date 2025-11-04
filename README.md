# 🧮 Calculator App

<div align="center">

A feature-rich Python calculator application with dual interfaces - a modern GUI and a powerful console mode, built using the MVC architecture pattern.

[![Python Version](https://img.shields.io/badge/python-3.x-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)
[![Tkinter](https://img.shields.io/badge/GUI-Tkinter-orange.svg)](https://docs.python.org/3/library/tkinter.html)

[Features](#-features) • [Installation](#-getting-started) • [Usage](#-usage) • [Architecture](#-architecture) • [Contributing](#-contributing)

</div>

---

## ✨ Features

### 🔢 Basic Operations
- ➕ **Addition** - Sum multiple numbers
- ➖ **Subtraction** - Calculate differences
- ✖️ **Multiplication** - Multiply values
- ➗ **Division** - Divide with zero-protection

### 🚀 Advanced Operations
- √ **Square Root** - Calculate square roots instantly
- 📊 **Percentage** - Quick percentage calculations
- 💾 **Memory Functions** - Store and recall values
  - `M+` Add to memory
  - `M-` Subtract from memory
  - Memory Store/Recall functionality

### 🎨 Dual Interface
- 🖥️ **GUI Mode** - Beautiful Tkinter-based interface with intuitive button layout
- 💻 **Console Mode** - Fast command-line interface for power users

## 📁 Project Structure

```
Calculator/
├── 📄 app.py                    # Main application entry point (GUI)
├── 📄 Calculator.py             # Console-based calculator
├── 📖 README.md                 # Project documentation
└── 📁 src/
    ├── __init__.py
    ├── 🎮 controller/
    │   ├── __init__.py
    │   └── calc_controller.py   # Controller logic (MVC)
    ├── 🧠 model/
    │   ├── __init__.py
    │   ├── simple_calc.py       # Core arithmetic operations
    │   └── special_calc.py      # Advanced operations & memory
    └── 🎨 view/
        ├── __init__.py
        └── Mainwindow.py        # Tkinter GUI implementation
```

## 🚀 Getting Started

### Prerequisites

- **Python 3.x** or higher
- **Tkinter** (included with standard Python installation)

> 💡 **No external dependencies required!** Everything uses Python's standard library.

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Devikrishna545/Calculator.git
   cd Calculator
   ```

2. **Verify Python installation**
   ```bash
   python --version  # Should show Python 3.x
   ```

3. **You're ready to go!** 🎉

### 🏃 Running the Application

#### GUI Calculator (Recommended for most users)
```bash
python app.py
```

#### Console Calculator (For command-line enthusiasts)
```bash
python Calculator.py
```

## 💡 Usage Guide

### 🖥️ GUI Interface

1. **Launch** the calculator: `python app.py`
2. **Click** number buttons to input values
3. **Select** an operation (+, -, ×, ÷, √, %)
4. **Press** `=` to see the result
5. **Clear** display with the `C` button

**Memory Operations:**
- `M+` - Add current display value to memory
- `M-` - Subtract current display value from memory
- `MR` - Recall stored memory value
- `MC` - Clear memory

### 💻 Console Interface

1. **Run** the console app: `python Calculator.py`
2. **Enter** your first number
3. **Choose** an operator:
   - `+` Addition
   - `-` Subtraction
   - `*` Multiplication
   - `/` Division
   - `sqt` Square root
   - `%` Percentage
4. **Specify** how many numbers to calculate (for basic operations)
5. **Enter** additional numbers as prompted
6. **Press** `=` to display the result

## 🏛️ Architecture

This project implements the **Model-View-Controller (MVC)** design pattern for clean separation of concerns:

### 📊 Component Breakdown

| Component | Location | Responsibility |
|-----------|----------|----------------|
| **Model** | `src/model/` | Business logic and calculations |
| **View** | `src/view/` | User interface rendering |
| **Controller** | `src/controller/` | Coordinates Model and View |

#### 🧠 Model Classes

**`SimpleCalculator`** - Basic Operations
```python
add(a, b)    # Addition
sub(a, b)    # Subtraction
mul(a, b)    # Multiplication
div(a, b)    # Division with zero-check
```

**`SpecialCalculator`** - Advanced Features
```python
sqrt(a)           # Square root calculation
perct(a)          # Percentage calculation
memory_store(c)   # Store value in memory
mem_recall()      # Retrieve memory value
mem_add(a)        # Add to memory
mem_sub(a)        # Subtract from memory
```

## 📚 Examples

### Basic Calculations
```python
15 + 25 = 40
100 - 30 = 70
8 × 7 = 56
84 ÷ 12 = 7.0
```

### Advanced Operations
```python
√16 = 4.0
25% of 200 = 50.0
```

### Memory Usage
```python
1. Calculate: 50 + 50 = 100
2. Press M+ (stores 100)
3. Calculate: 25 × 2 = 50
4. Press MR (recalls 100)
5. Add recalled value to current
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork** the repository
2. **Create** a feature branch
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Commit** your changes
   ```bash
   git commit -m 'Add some amazing feature'
   ```
4. **Push** to the branch
   ```bash
   git push origin feature/amazing-feature
   ```
5. **Open** a Pull Request

### 🐛 Found a Bug?
Please [open an issue](https://github.com/Devikrishna545/Calculator/issues) with details about the problem.

## 🎯 Future Roadmap

- [ ] 🔬 Scientific functions (sin, cos, tan, log, exp)
- [ ] 📜 Calculation history viewer
- [ ] ⌨️ Keyboard input support for GUI
- [ ] 🧪 Comprehensive unit tests
- [ ] 🎨 Theme customization (Dark mode, Light mode)
- [ ] 📊 Graphing capabilities
- [ ] 🌐 Multi-language support
- [ ] 💾 Export calculation history

## ⚠️ Known Limitations

- Console interface multi-number operations need refinement
- Enhanced error messages for edge cases in development
- GUI keyboard shortcuts not yet implemented

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Devikrishna545**
- 🐙 GitHub: [@Devikrishna545](https://github.com/Devikrishna545)
- 📧 Feel free to reach out for questions or suggestions!

## 🙏 Acknowledgments

- Built with Python's powerful standard library
- GUI powered by Tkinter
- Inspired by classic calculator designs

---

<div align="center">

**⭐ If you found this project useful, please consider giving it a star!**

Made with ❤️ by Devikrishna545

</div>
