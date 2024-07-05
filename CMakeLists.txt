cmake_minimum_required(VERSION 3.10)

# 项目信息
project(cpp-project VERSION 1.0)

# 设置 C++ 标准
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# 在项目目录下的 include 目录中查找头文件，这些头文件定义了类、函数原型等
include_directories(include)

# 查找所有源文件
file(GLOB SOURCES "src/*.cpp")

# 生成可执行文件
add_executable(cpp-project ${SOURCES})

