cmake_minimum_required(VERSION 3.0.0)

project(libdoomtools VERSION 1.0)
set(CMAKE_STATIC_LIBRARY_PREFIX "")

set(SOURCES
    src/cmdlib.c)

add_library(libdoomtools STATIC ${SOURCES})

target_include_directories(libdoomtools
    PUBLIC
        ${PROJECT_SOURCE_DIR}/include
)
