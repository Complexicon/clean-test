cmake_minimum_required(VERSION 3.1)

set(CMAKE_BUILD_TYPE Debug)
set(CMAKE_CXX_STANDARD_REQUIRED 17)

project("template" VERSION 1.0.0)


file(GLOB_RECURSE source_list "src/*.cpp")
include_directories(${CMAKE_SOURCE_DIR}/include)
add_executable(out ${source_list})