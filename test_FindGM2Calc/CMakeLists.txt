cmake_minimum_required(VERSION 2.8.12)
project(TestFindGM2Calc)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED YES)
set(CMAKE_C_STANDARD 99)
set(CMAKE_C_STANDARD_REQUIRED YES)

find_package(Boost 1.37.0 REQUIRED)
find_package(Eigen3 3.1 REQUIRED)
find_package(GM2Calc REQUIRED)

include_directories(${EIGEN3_INCLUDE_DIR})

add_executable(example-cpp example.cpp)
target_link_libraries(example-cpp GM2Calc::GM2Calc)

add_executable(example-c example.c)
target_link_libraries(example-c GM2Calc::GM2Calc m stdc++)
