# ANSI String Formatter

A Python utility for formatting terminal output with ANSI escape codes, providing support for colors, font styles, and text formatting.

## Features

- 🎨 **Color Support**: Foreground and background colors
- 📝 **Font Styling**: Bold, thin, italics, underline, strikethrough
- 🌈 **Multiple Color Formats**: String names, RGB tuples, 256-color codes
- 🔧 **Easy to Use**: Simple function interface

## Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/ansi-string-formatter.git

# Or simply download the string_format.py file
```
## Examples
```python
from string_format import string_formatter

# Basic usage with color names
formatted_text = string_formatter("Hello World", fg_color="red", bold=True)
print(formatted_text)

# Using RGB values
formatted_text = string_formatter("Colorful Text", fg_color=(255, 0, 255), bg_color=(50, 50, 50))
print(formatted_text)

# Multiple styles
formatted_text = string_formatter(
    "Styled Text", 
    fg_color="blue", 
    bold=True, 
    underline=True, 
    italics=True
)
print(formatted_text)
```

## API Reference

### `string_formatter(string, **kwargs)`

Main function for formatting strings with ANSI escape codes.

**Parameters:**
- `string` (str): The input string to format
- `bg_color` (str|int|tuple, optional): Background color
- `fg_color` (str|int|tuple, optional): Foreground color
- `bold` (bool): Apply bold formatting
- `thin` (bool): Apply thin formatting
- `italics` (bool): Apply italic formatting
- `underline` (bool): Apply underline formatting
- `strikethrough` (bool): Apply strikethrough formatting

**Returns:**
- `str`: Formatted string with ANSI escape codes

## Dependencies

- `functools` (Python standard library)

## License

MIT License
