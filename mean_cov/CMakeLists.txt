cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

add_definitions(-std=c++11)

set(CXX_FLAGS "-Wall" "-pedantic")
set(CMAKE_CXX_FLAGS, "${CXX_FLAGS}")

project(camera_fusion)

include_directories(/usr/include/eigen3)

# Executable for create matrix exercise
add_executable (mean_cov mean_cov.cpp ukf.cpp)