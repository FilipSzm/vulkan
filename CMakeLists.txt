cmake_minimum_required(VERSION 3.21)
project(Vulkan)

set(CMAKE_CXX_STANDARD 23)

include_directories(include)
link_directories(lib)

find_package(Vulkan REQUIRED)

add_executable(Vulkan main.cpp)

target_link_libraries(Vulkan glfw3 Vulkan::Vulkan)

