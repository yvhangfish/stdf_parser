cmake_minimum_required(VERSION 3.12)
project(libstdf C)

set(CMAKE_C_STANDARD 99)

include_directories(../include)

aux_source_directory(. SRC)
add_library(libstdf ${SRC})