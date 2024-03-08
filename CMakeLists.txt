cmake_minimum_required(VERSION 3.5.0)

project(argtable3 "C")

set(src "argtable3.c")
set(inc ${CMAKE_CURRENT_SOURCE_DIR})
set(priv_inc ${inc}/argtable3)

add_library(${PROJECT_NAME} ${src})
target_include_directories(${PROJECT_NAME} PUBLIC  ${inc})
target_include_directories(${PROJECT_NAME} PRIVATE ${priv_inc})
