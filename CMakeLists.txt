cmake_minimum_required(VERSION 2.8)

project(HelloWorld CXX)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pedantic -Wall -Wextra")
set(CMAKE_CXX_FLAGS_DEBUG "${CMAKE_CXX_FLAGS_DEBUG} -O0 -g")

file(GLOB SRC_LIST
    "src/*.h"
    "src/*.cpp"
)
add_executable(${PROJECT_NAME} ${SRC_LIST})
