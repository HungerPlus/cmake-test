cmake_minimum_required(VERSION 3.16)
PROJECT(test1)

aux_source_directory(./ SRC)
include_directories(${CURR_DIR}/application ${CURR_DIR}/interface) #包含头文件路径
link_directories(${LIBPATH})
link_libraries(app)
set(EXECUTABLE_OUTPUT_PATH ${BINPATH})

add_executable(app_hello ${SRC})
