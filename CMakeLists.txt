cmake_minimum_required(VERSION 3.15)
project(todo-fltk)

set(CMAKE_CXX_STANDARD 17)

# Enable CMake integration with vcpkg
find_package(FLTK REQUIRED NO_MODULE)

add_executable(todo main.cpp)

target_link_libraries(todo PRIVATE FLTK::FLTK)
