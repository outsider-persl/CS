# Office Document

 [Reference Documentation](https://cmake.org/cmake/help/latest/)
#  Template

```c
cmake_minimum_required(VERSION 3.15...3.30)

  

project(dsa_cpp VERSION 1.0

DESCRIPTION "DSA in C++"

LANGUAGES CXX)

# 设置 C++ 标准

set(CMAKE_CXX_STANDARD 17) # 使用 C++17

set(CMAKE_CXX_STANDARD_REQUIRED ON) # 确保该标准是必需的

set(CMAKE_CXX_EXTENSIONS OFF) # 禁用扩展，使用标准 C++

  

# 包含 include 目录中的头文件

include_directories(${PROJECT_SOURCE_DIR}/include)

# 查找源文件

file(GLOB SOURCES "src/*.cpp")

  

# 定义输出目录

set(EXECUTABLE_OUTPUT_PATH ${CMAKE_SOURCE_DIR}/bin)

  

# 添加可执行文件

# add_executable(dsa_cpp ${SOURCES})

add_executable(exec src/move_func.cpp)
```