cmake_minimum_required(VERSION 3.5)

project(mywebserver LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(SOURCES
    src/main_http.cpp
    )

find_package(Boost REQUIRED)

include_directories(${Boost_INCLUDE_DIRS})

target_link_libraries(mywebserver ${Boost_LIBRARIES})

add_executable(mywebserver ${SOURCES})
