#set the minimum required version of cmake
cmake_minimum_required(VERSION 3.15)

#naming the project
project(mathemathics_tool_for_derivation_and_integration VERSION 1.0)

#set standards
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

#enable testing in ordert to allow test with Gtest
enable_testing()

#adding subdirectories
add_subdirectory(src)
add_subdirectory(tests)