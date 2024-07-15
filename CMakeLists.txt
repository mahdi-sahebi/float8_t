cmake_minimum_required(VERSION 3.2 FATAL_ERROR)
project(float8 LANGUAGES CXX VERSION 1.0.0)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

include_directories(${CMAKE_CURRENT_SOURCE_DIR})

add_subdirectory(elb)
add_subdirectory(tests)
