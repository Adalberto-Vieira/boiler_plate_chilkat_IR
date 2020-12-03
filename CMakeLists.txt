cmake_minimum_required(VERSION 3.10)
project(crawler)

set(SOURCE_FILES crawler.cpp)

INCLUDE_DIRECTORIES(include)
LINK_DIRECTORIES(lib)

add_executable(crawler ${SOURCE_FILES})

target_link_libraries(${PROJECT_NAME} libchilkat-9.5.0.so)

