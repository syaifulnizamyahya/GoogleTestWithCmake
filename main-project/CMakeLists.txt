# CMakeList.txt : CMake project for autogtest, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.8)

# Add source to this project's executable.
add_executable (main-project "main.cpp" "main.h")

# link to library
target_link_libraries (main-project Sqr)
