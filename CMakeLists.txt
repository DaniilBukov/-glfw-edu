cmake_minimum_required(VERSION 3.13 FATAL_ERROR)

project(OpenGL-edu)

add_executable(OpenGL-edu src/main.cpp)

set(GLFW_BUILD_DOCS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_TESTS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_EXAMPLES OFF CACHE BOOL "" FORCE)
add_subdirectory(external/glfw)

target_link_libraries(OpenGL-edu glfw)