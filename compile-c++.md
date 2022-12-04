1. Download CMake: https://cmake.org/download/
2. Download MinGw: https://sourceforge.net/projects/mingw/files/Installer/mingw-get/
3. Add CMake to path (envt variables -> path -> new -> paste path)
4. Add bin folder of MinGW to path
5. Open terminal and run ```mingw-get install mingw-gcc-g++```

Actually building with cmake:
1. Go to dir in terminal where CMakeList.txt is
2. Run the following command ```cmake -S . -B ./build -G "MinGW Makefiles"```
3. Go to build dir
4. Run the following command ```cmake --build . --config Debug``` or for release ```cmake --build . --config Release``` to build .exe file
