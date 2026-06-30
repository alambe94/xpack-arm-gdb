# Standalone xPack GNU Arm GDB for Windows x64

This repository contains a lightweight, standalone build of `arm-none-eabi-gdb` (GDB 14.2) extracted from the official [xPack GNU Arm Embedded GCC](https://github.com/xpack-dev-tools/arm-none-eabi-gcc-xpack) release.

## Features

- **Lightweight**: Only **~35 MB** total, compared to the full toolchain download of ~265 MB (and ~400 MB extracted).
- **XML / Expat Support**: Fully supports XML target descriptions from OpenOCD / GDB Server (resolving GDB packet truncation errors like `Truncated register 16 in remote 'g' packet`).
- **Python 3 Support**: Includes Python scripting support and standard scripts (`share/gdb`).

## Extraction Source

Extracted from:
- **Archive**: `xpack-arm-none-eabi-gcc-13.3.1-1.1-win32-x64.zip`
- **Compiler Version**: GCC 13.3.1-1.1
- **GDB Version**: GDB 14.2.90.20240526-git

## Contents

- `bin/arm-none-eabi-gdb.exe` - Standalone GDB executable
- `bin/arm-none-eabi-gdb-py3.exe` - Python-enabled GDB executable
- `bin/python311.zip` & `bin/*.dll` - Required runtime dependencies
- `arm-none-eabi/share/gdb/` - Standard python integration scripts

## License

This project distributes binary executables compiled from the GNU Project Debugger (GDB), which is licensed under the [GNU General Public License v3 (GPLv3)](LICENSE).
