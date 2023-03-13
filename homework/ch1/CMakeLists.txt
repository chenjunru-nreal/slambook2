cmake_minimum_required(VERSION 3.12)

project(helloSLAM)

include_directories("include")

# only focus on source file, compiler will handler header file
add_library(libHello SHARED src/hello.cpp)
 
add_executable(say_hello main.cpp)
target_link_libraries(say_hello libHello)