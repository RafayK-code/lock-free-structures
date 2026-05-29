cmake_minimum_required(VERSION 3.20)
project(atomic_stack)

if(CMAKE_SOURCE_DIR STREQUAL CMAKE_CURRENT_SOURCE_DIR)
    set(CMAKE_CXX_STANDARD 20)
    set(CMAKE_CXX_STANDARD_REQUIRED ON)
    set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
endif()

add_library(atomic_stack INTERFACE)
target_include_directories(atomic_stack INTERFACE .)
target_compile_features(atomic_stack INTERFACE cxx_std_20)
