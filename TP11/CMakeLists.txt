cmake_minimum_required(VERSION 3.10)
project(aeda1920_fp11_sol)

set(CMAKE_CXX_STANDARD 11)

add_subdirectory(lib/googletest-master)
include_directories(lib/googletest-master/googletest/include)
include_directories(lib/googletest-master/googlemock/include)

add_executable(aeda1920_fp11_sol main.cpp Tests/tests.cpp Tests/disjointSets.cpp Tests/maze.cpp)

target_link_libraries(aeda1920_fp11_sol gtest gtest_main)