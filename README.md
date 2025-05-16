# INFOMOV Assignment 1

## Setup
If you are on windows:
* Run the `bootstrap_windows.bat` file (this requires Visual Studio 17 2022 by default).
* Open the generated Visual Studio project located in the build folder.
* Run the project in Release mode, making sure you select GAME as the build target.
  
If you are on Linux/Mac:
* Depending on your architecture, run either `bootstrap_linux_mac_x86.sh` or `bootstrap_linux_mac_ARM.sh` (making sure you can run it using `chmod +x bootstrap_linux_mac_*.sh`)
* In your build folder you can now run `make` in the future if you want to recompile after making changes to the code.
* Execute `./GAME` to run the project (making sure you can run it using `chmod +x GAME`)

## Expected Grade

7

## Changes

- Precomputed gray interpolation factor, because it was the same for all 3 channels.
- Rewrote color computations to use integer approximations
- Replaced divisions and other expensive operations with bitwise operations
- Replace branch instructions with bitwise operations or multiplications with comparisons
- Replaced array access with pointer arithmetic
- Replaced long and doubles with shorts and floats
- Changed compiler flags to optimize for speed