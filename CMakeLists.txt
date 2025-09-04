cmake_minimum_required(VERSION 3.15)

project(blackhole LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(OpenGL REQUIRED)
find_package(GLEW REQUIRED)

add_executable(blackhole blackhole.cpp)

target_link_libraries(blackhole PRIVATE GLEW::GLEW OpenGL::GL)
