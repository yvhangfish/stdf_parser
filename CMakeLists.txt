cmake_minimum_required(VERSION 3.12)
project(stdf)

set(CMAKE_CXX_STANDARD 14)

include_directories(./include)

add_subdirectory(libstdf)

aux_source_directory(. SRC)
add_executable(stdfParser ${SRC})
target_link_libraries(stdfParser libstdf)