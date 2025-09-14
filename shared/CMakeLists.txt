cmake_minimum_required(VERSION 3.14)

project(shared)

add_library(shared STATIC
        dart-sdk/include/dart_api_dl.c
)

target_include_directories(shared PUBLIC
        ${CMAKE_CURRENT_SOURCE_DIR}
        ${CMAKE_CURRENT_SOURCE_DIR}/dart-sdk/include
)