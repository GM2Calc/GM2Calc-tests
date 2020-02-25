cmake_minimum_required(VERSION 2.8.12)
project(TestSubproject)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED YES)
set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED YES)

add_subdirectory(GM2Calc)

add_executable(example-cpp example.cpp)
target_link_libraries(example-cpp GM2Calc::GM2Calc)

add_executable(example-c example.c)
target_link_libraries(example-c GM2Calc::GM2Calc m stdc++)
