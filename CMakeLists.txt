cmake_minimum_required(VERSION 3.7)
project(TextFlow)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES main.cpp TextFlow_Tests.cpp TextFlow.hpp Surrogate.cpp)
add_library(TextFlow INTERFACE TextFlow.hpp)
target_include_directories(TextFlow INTERFACE ${CMAKE_CURRENT_LIST_DIR})
#add_executable(TextFlowTest ${SOURCE_FILES})
