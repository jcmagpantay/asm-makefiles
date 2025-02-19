# ASM Makefiles
[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## About
This repository provides examples and templates for using Makefiles with Assembly (ASM) projects. Makefiles are powerful build automation tools that simplify the compilation and linking process, making ASM development more efficient and organized.

## What are Makefiles?
Makefiles are scripts that automate the build process by defining rules for compiling and linking source files. They help manage dependencies between files and ensure only modified files are recompiled, saving development time.

Key benefits for ASM development:
- Automate repetitive assembly and linking commands
- Handle multiple source files efficiently
- Maintain consistent build processes across different environments
- Enable easy inclusion of debugging symbols and optimization flags
- Support different build configurations (debug/release)

## Getting Started

### Prerequisites
- NASM (Netwide Assembler) or your preferred assembler
- GNU Make
- A C linker (usually gcc or ld)

## Common Make Commands
- `make`: Build the default target
- `make debug`: Build with debugging information
- `make clean`: Remove all generated files
- `make -j4`: Parallel build using 4 cores

## Tips for ASM Development
1. Use separate source files for different functionalities
2. Keep common macros and constants in include files
3. Enable debugging symbols during development
4. Use meaningful labels and comments
5. Maintain consistent naming conventions

## Contributing
Contributions are welcome! Please feel free to submit pull requests.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments
- NASM documentation team
- GNU Make documentation
- Assembly programming community

## Contact
John Michael C. Magpantay - [@jcmagpantay](https://linkedin.com/in/jm-magpantay)
Project Link: [https://github.com/jcmagpantay/asm-makefiles](https://github.com/jcmagpantay/asm-makefiles)
