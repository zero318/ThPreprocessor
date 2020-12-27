# CMakeList.txt : CMake project for ThPreprocessor, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

project("ThPreprocessor" VERSION 0.1.0.0 LANGUAGES NONE)
enable_language(C)
SET(CMAKE_C_FLAGS  "${CMAKE_C_FLAGS} -Xclang -std=c2x")
include_directories("F:\\Program Files (x86)\\LLVM\\lib\\clang\\12.0.0\\include")

# Add source to this project's executable.
add_executable (ThPreprocessor "ThPreprocessor.c" "ThPreprocessor.h")

# TODO: Add tests and install targets if needed.
