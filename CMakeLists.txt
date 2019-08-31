cmake_minimum_required(VERSION 3.0.0)
project(tinyraycaster VERSION 0.1.0)

include(CTest)
enable_testing()

add_executable(tinyraycaster tinyraycaster.cpp)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)

# The following folder will be included
include_directories("${PROJECT_SOURCE_DIR}")

# Set the output folder where your program will be created
set(CMAKE_BINARY_DIR ${CMAKE_SOURCE_DIR}/bin)
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR})
set(LIBRARY_OUTPUT_PATH ${CMAKE_BINARY_DIR})