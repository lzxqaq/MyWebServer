cmake_minimum_required(VERSION 3.5)

project(mywebserver LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(SOURCES
    src/main_http.cpp
    )

add_executable(mywebserver ${SOURCES})
