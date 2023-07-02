cmake_minimum_required(VERSION 3.25)
project(raylib-imgui-cmake)

find_package(raylib 4.0 REQUIRED) # Requires at least version 3.0
find_package(imgui)
set(CMAKE_C_STANDARD 11) # Requires C11 standard

set(CMAKE_CXX_STANDARD 17)


add_executable(${PROJECT_NAME} src/main.cpp src/rlImGui.cpp)

target_link_libraries(${PROJECT_NAME} raylib imgui)

