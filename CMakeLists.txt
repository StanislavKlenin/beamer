project(LOGGER)
cmake_minimum_required(VERSION 2.6)

set(CMAKE_CXX_FLAGS "--std=c++11 -Wall")
set(LIBRARY_OUTPUT_PATH    ${CMAKE_BINARY_DIR}/lib)

add_library(logger logger.cpp file.cpp)

target_include_directories(logger PRIVATE "${CMAKE_CURRENT_SOURCE_DIR}")
