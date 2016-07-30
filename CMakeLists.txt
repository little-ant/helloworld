cmake_minimum_required(VERSION 3.0)
project (helloworld)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wextra")

add_executable(hello helloworld.cpp)
