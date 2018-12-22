cmake_minimum_required(VERSION 3.7)

set(PROJECT_NAME ra-common)
project(${PROJECT_NAME})

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)

file(GLOB SRC src/*.cpp)

add_library(${PROJECT_NAME} ${SRC})

target_include_directories(${PROJECT_NAME} PUBLIC include)