cmake_minimum_required(VERSION 3.10)
project(TodoApp)

find_package(FLTK REQUIRED)

add_executable(todo main.cpp)
target_link_libraries(todo fltk)
