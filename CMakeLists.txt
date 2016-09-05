project(SOIL2)
cmake_minimum_required(VERSION 2.6)

set(SOURCE_DIR src/SOIL2)

add_subdirectory(${SOURCE_DIR})

get_directory_property(HAS_PARENT PARENT_DIRECTORY)
if (HAS_PARENT)
    set(SOIL2_INCLUDE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/${SOURCE_DIR} PARENT_SCOPE)
endif ()