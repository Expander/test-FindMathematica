cmake_minimum_required(VERSION 3.1)
project(test-FindMathematica LANGUAGES CXX Fortran)

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} ${PROJECT_SOURCE_DIR}/cmake)

find_package(Mathematica 8.0)

if(Mathematica_FOUND)
  Mathematica_ADD_LIBRARY(mylib ${PROJECT_SOURCE_DIR}/src/mylib.cpp)
endif()
