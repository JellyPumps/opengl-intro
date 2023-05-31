cmake_minimum_required(VERSION 3.1 FATAL_ERROR)

project(
    glad
    VERSION 1.0
    LANGUAGES CXX
)

add_library(glad "src/glad.c")

target_include_directories(glad SYSTEM PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include")