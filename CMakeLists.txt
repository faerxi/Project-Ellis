cmake_minimum_required(VERSION 3.27)
project(Elysia VERSION 0.1)

set(CMAKE_CXX_STANDARD 23)

set(PROJECT_SOURCE_DIR Source)
set(ELYSIA_HEADER_DIR ${PROJECT_SOURCE_DIR}/include/elysia)
set(ELYSIA_SOURCE_DIR ${PROJECT_SOURCE_DIR}/src/elysia)

add_executable(Elysia ${PROJECT_SOURCE_DIR}/main.cpp)
target_include_directories(Elysia PUBLIC ${PROJECT_SOURCE_DIR}/include)
target_compile_options(Elysia PRIVATE -Wall -Wextra -Wpedantic -Wconversion -Wunused -Werror)
