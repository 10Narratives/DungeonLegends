cmake_minimum_required(VERSION 3.15...3.30 FATAL_ERROR)

set(PROJECT_NAME DungeonLegends)
project(${PROJECT_NAME}
        VERSION 0.0.0
        DESCRIPTION "Simple game written in C++"
        HOMEPAGE_URL ""
        LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
# TODO: setup debug and release sets of flags
# set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wextra")
set(CMAKE_EXPORT_COMPILE_COMMANDS TRUE)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

add_executable(${PROJECT_NAME} main.cc)
