cmake_minimum_required(VERSION 3.3)
project (helloworld)

# set executeable name
set(PRG_NAME tqt)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wextra")

set(CMAKE_BUILD_TYPE Debug)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_CXX_COMPILER /usr/bin/g++)

find_package( Threads )
add_executable(${PRG_NAME} helloworld.cpp)

target_link_libraries(${PRG_NAME} ${CMAKE_THREAD_LIBS_INIT})
