cmake_minimum_required(VERSION 3.17 FATAL_ERROR)
project(ElaborateLib LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

include_directories(${CMAKE_CURRENT_SOURCE_DIR})

add_subdirectory(elb)
add_subdirectory(tests)
