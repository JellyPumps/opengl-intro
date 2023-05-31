cmake_minimum_required(VERSION 3.1 FATAL_ERROR)

project(
    openglApp
    VERSION 1.0
    LANGUAGES CXX
)

add_subdirectory(glad)
target_include_directories(openglApp PRIVATE glad)

set(SOURCES "src/main.cpp")

add_executable(openglApp ${SOURCES})