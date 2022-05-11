cmake_minimum_required(3.20.6)
project(tinykv)

file(tinykv_sources ${PROJECT_SOURCE_DIR}/src/*/*.cpp ${PROJECT_SOURCE_DIR}/src/*/*/*.cpp)
add_library(tinykv_shared ${tinykv_sources})

file(Sources ${PROJECT_SOURCE_DIR}/src/*/*.cpp)
file(Headers ${PROJECT_SOURCE_DIR}/src/include/*.h)
add_executable(tinykv )
