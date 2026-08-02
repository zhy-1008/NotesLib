# 生成库文件
add_library(core core/core.cpp)

# 生成可执行文件
add_executable(NotesLib cli/main.cpp)

# 链接库文件，添加依赖关系
target_link_libraries(NotesLib core)