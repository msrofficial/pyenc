# Python File Obfuscator

A Python script that obfuscates Python source code files using marshal serialization to protect intellectual property.

## Features

- Converts Python source code into marshaled bytecode
- Preserves script functionality while making source unreadable
- Simple command-line interface
- Shows user geolocation information (IP and country)
- Cross-platform compatibility (Windows/Linux/macOS)

## Installation

1. Clone this repository:
```bash
git clone https://github.com/msrofficial/python-obfuscator.git
cd python-obfuscator
```

2. Ensure you have Python 3.x installed:
```bash
python3 --version
```

3. Install required dependencies:
```bash
pip install requests
```

## Usage

Run the obfuscator:
```bash
python3 enc.py
```

Follow the on-screen prompts:
1. Enter the path to the Python file you want to obfuscate
2. Specify the output file name
3. The script will generate an obfuscated version of your file

Example output file structure:
```python
#!/usr/bin/env python3
# Obfuscated By MSR
import marshal
exec(marshal.loads(b'\x63\x00\x00\x00...'))  # marshaled bytecode
```

## How It Works

The obfuscator:
1. Reads your Python source file
2. Compiles it into Python bytecode
3. Serializes the bytecode using Python's `marshal` module
4. Generates a new Python file that loads and executes the marshaled bytecode

## Limitations

- Works only with Python code
- Obfuscated files are slightly larger than original
- Requires Python environment to run

## Disclaimer

This tool is intended for educational purposes and protecting intellectual property. Please use responsibly and in compliance with all applicable laws. The author is not responsible for any misuse of this software.

## Author

**Sakibur Rahman (MSR)**
- Website: [https://msrsakibur.netlify.app](https://msrsakibur.netlify.app)
- GitHub: [https://github.com/msrofficial](https://github.com/msrofficial)
- Facebook: [https://www.facebook.com/sakibur.msr](https://www.facebook.com/sakibur.msr)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
