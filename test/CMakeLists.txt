cmake_minimum_required(VERSION 3.20)
project(test)

set(CMAKE_CXX_STANDARD 17)

find_package(Catch2)
if(Catch2_FOUND)
    set(EXECUTABLE_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/out/${MY_BUILD_NAME}/test/)
    add_subdirectory(lib)
endif()
