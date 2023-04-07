cmake_minimum_required(VERSION 3.24)
project(untitled)

set(CMAKE_CXX_STANDARD 17)

add_executable(untitled main.cpp)

# Adding compiler flag /we4067 breaks project load
# Commenting it out fixes configuration
target_compile_options(untitled PUBLIC /we4067)
