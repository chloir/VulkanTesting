cmake_minimum_required(VERSION 3.15)
project(VulkanTesting)

set(CMAKE_CXX_STANDARD 17)

include_directories(/usr/local/include)
include_directories(/Users/kumac/Documents/vulkansdk-macos-1.1.130.0/macOS/include)

link_directories(/usr/local/lib)
link_directories(/Users/kumac/Documents/vulkansdk-macos-1.1.130.0/macOS/lib)

add_executable(VulkanTesting main.cpp)

target_link_libraries(VulkanTesting /usr/local/lib/libglfw.3.3.dylib)
target_link_libraries(VulkanTesting /Users/kumac/Documents/vulkansdk-macos-1.1.130.0/macOS/lib/libvulkan.1.dylib)
target_link_libraries(VulkanTesting /Users/kumac/Documents/vulkansdk-macos-1.1.130.0/macOS/lib/libvulkan.1.1.130.dylib)