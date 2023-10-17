## Dependencies

-   CMake Installation
-   Conan Installation
-  Install Microsoft Visual C++ and MSBuild Tools packages

# Compiling and Running

## On Linux

- Run `conan install . --build=missing` at the root of your build directory
- Install the missing packages
- Create the directory "build" and go in
- Run `cmake .. -DCMAKE_BUILD_TYPE=Release` and after that run `make`

## On Windows

- Configure the Path for MSBuild Tools
- Run `conan install . --build=missing -of=build` at the root of your build directory
- Enter in the build directory with `cd build`
- Run `cmake .. -DCMAKE_BUILD_TYPE=Release -G "Visual Studio 17"`
- Run `cmake --build . --config Release`