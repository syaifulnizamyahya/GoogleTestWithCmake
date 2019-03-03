# CMakeList.txt : Top-level CMake project file, do global configuration
# and include sub-projects here.
#
cmake_minimum_required (VERSION 3.8)

project ("GoogleTestWithCmake")

# main project
add_subdirectory ("main-project")
# library used by main project
add_library (Sqr sqr/sqr.cpp sqr/sqr.h)

# test project 
enable_testing()
add_subdirectory ("test")
add_test(NAME MyTest COMMAND Test)