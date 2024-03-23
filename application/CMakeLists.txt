cmake_minimum_required(VERSION 3.16)
project(application)
aux_source_directory(./ SRC) #查找源文件路径

include_directories(${PROJECT_SOURCE_DIR}) #包含头文件路径
set(LIBRARY_OUTPUT_PATH ${LIBPATH}) #设置库文件保存路径
add_library(app STATIC ${SRC}) #设置库文件名字 编译成静态库