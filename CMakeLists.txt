cmake_minimum_required(VERSION 3.28)
project(untitled1)

set(CMAKE_CXX_STANDARD 20)

find_package(Vulkan REQUIRED)
include_directories("E:/glfw-3.4.bin.WIN64/include")
include_directories("E:/glm")
include_directories("C:/VulkanSDK/1.3.290.0/Include")


set(GLFW_DIR "E:/glfw-3.4.bin.WIN64/")


add_executable(untitled1 main.cpp
)

target_include_directories(untitled1 PRIVATE "E:/glfw-3.4.bin.WIN64/include")
target_include_directories(untitled1 PRIVATE "E:/glm")




target_link_libraries(untitled1 Vulkan::Vulkan ${GLFW_DIR}/lib-mingw-w64/libglfw3.a)





