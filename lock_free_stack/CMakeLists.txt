cmake_minimum_required(VERSION 3.20)
project(lock_free_stack)

if(CMAKE_SOURCE_DIR STREQUAL CMAKE_CURRENT_SOURCE_DIR)
    set(CMAKE_CXX_STANDARD 20)
    set(CMAKE_CXX_STANDARD_REQUIRED ON)
    set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
endif()

add_library(lock_free_stack INTERFACE)
target_include_directories(lock_free_stack INTERFACE .)
target_compile_features(lock_free_stack INTERFACE cxx_std_20)