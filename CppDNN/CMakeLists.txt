cmake_minimum_required(VERSION 2.8)

project(EigenDNN)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++0x")

find_package (Eigen3 3.3 REQUIRED NO_MODULE)

set(CMAKE_BUILD_TYPE Release)
 
file(GLOB HEADERS "*.h")
 
install (FILES ${HEADERS} DESTINATION /usr/local/include/CppDNN)
