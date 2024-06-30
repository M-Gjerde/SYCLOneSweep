cmake_minimum_required(VERSION 3.22)
project(OneSweepSYCL)

set(CMAKE_CXX_COMPILER "clang++")
set(CMAKE_CXX_FLAGS "-fsycl -fsycl-targets=nvptx64-nvidia-cuda -g")
set(CMAKE_CXX_STANDARD 17)

add_executable(onesweep_sycl main.cpp)