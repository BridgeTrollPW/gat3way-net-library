cmake_minimum_required(VERSION 3.0.0)
project(gat3way-net-library VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 17)

include(CTest)
enable_testing()

add_library(gat3way-net-library 
sources/WebServer.cpp)

target_include_directories(gat3way-net-library  PRIVATE includes)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)
