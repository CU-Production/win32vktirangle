cmake_minimum_required(VERSION 3.27)
project(win32vktirangle)

set(CMAKE_CXX_STANDARD 17)

find_package(Vulkan REQUIRED)

add_executable(triangle main.c)
target_link_libraries(triangle PRIVATE Vulkan::Vulkan)
