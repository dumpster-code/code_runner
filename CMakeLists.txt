cmake_minimum_required(VERSION 3.10)

project(CodeRunner VERSION 1.0 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_executable(${PROJECT_NAME} src/main.cpp)

add_subdirectory(third_party/googletest)
include_directories(third_party/googletest/googletest/include)

add_subdirectory(tests)
