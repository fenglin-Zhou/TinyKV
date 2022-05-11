cmake_minimum_required(3.20.6)

project(TinyKV)

aux_source_directory(. DIR_SRCS)

add_subdirectory(src)

add_executable(server server.cpp)
target_link_libraries(server )