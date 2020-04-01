cmake_minimum_required(VERSION 3.10)

# set the project name
project(CppSandboxTests)

set(THREADS_PREFER_PTHREAD_FLAG ON)
find_package(Threads REQUIRED)

include_directories("/home/khuston/dependencies/googletest/googletest/include/")

link_directories("/home/khuston/dependencies/googletest/googletest/build/lib/")

add_executable(CppSandboxTests tests/test.cpp)

target_link_libraries(CppSandboxTests gtest)
target_link_libraries(CppSandboxTests gtest_main)
target_link_libraries(CppSandboxTests Threads::Threads)