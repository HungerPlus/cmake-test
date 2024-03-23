cmake_minimum_required(VERSION 3.16)
PROJECT(hello)
message(${PROJECT_SOURCE_DIR})

set(CURR_DIR ${PROJECT_SOURCE_DIR})
set(LIBPATH ${PROJECT_SOURCE_DIR}/lib)
set(BINPATH ${PROJECT_SOURCE_DIR}/bin)

add_subdirectory(application)
add_subdirectory(interface)
add_subdirectory(test1)


