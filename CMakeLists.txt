cmake_minimum_required(VERSION 3.8)
project(nethogs)

SET(CMAKE_C_COMPILER /usr/local/bin/gcc-7)
SET(CMAKE_CXX_COMPILER /usr/local/bin/g++-7)
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
#message(${PROJECT_SOURCE_DIR})
#message(${PROJECT_BINARY_DIR})
#message(${CMAKE_MAKE_PROGRAM})
#message(STATUS ${WIN32})
add_custom_target(nethogs ALL COMMAND ${CMAKE_MAKE_PROGRAM} -C ${PROJECT_SOURCE_DIR}
        CLION_EXE_DIR=${PROJECT_BINARY_DIR})
#add_executable(nethogs ${nethogs_SOURCE_DIR}/src/nethogs)