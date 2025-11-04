cmake_minimum_required (VERSION 3.20)

file(GLOB_RECURSE SUBDIRECTORIES "${CMAKE_SOURCE_DIR}/Source/*.h" "${CMAKE_SOURCE_DIR}/Source/*.cpp")
source_group("Source" "${CMAKE_SOURCE_DIR}/Source" ${SUBDIRECTORIES})		
add_executable (DirectXFantasy main.cpp ${SUBDIRECTORIES})

target_include_directories(DirectXFantasy PRIVATE "${CMAKE_SOURCE_DIR}/Source")
