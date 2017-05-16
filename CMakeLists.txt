cmake_minimum_required(VERSION 3.8)
project(nethogs)

SET(CMAKE_C_COMPILER /usr/local/bin/gcc-7)
SET(CMAKE_CXX_COMPILER /usr/local/bin/g++-7)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

add_custom_target(nethogs ALL COMMAND gmake -C ${nethogs_SOURCE_DIR}
        CLION_EXE_DIR=${PROJECT_BINARY_DIR})