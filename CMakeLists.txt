# cmake最低版本
cmake_minimum_required(VERSION 3.10)

# 设置编译器路径
set(CMAKE_CXX_COMPILER "E:/MSYS2/ucrt64/bin/g++.exe")

# 项目名称
project(NotesLib CXX)

# 生成compile_commands.json文件
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

# 强制要求编译器必须支持指定的C++标准版本
set(CMAKE_CXX_STANDARD_REQUIRED ON)
# 禁用编译器的非标准语言扩展
set(CMAKE_CXX_EXTENSIONS OFF)
# c++标准
set(CMAKE_CXX_STANDARD 20)

# 添加子目录
add_subdirectory(src)
add_subdirectory(tests)


