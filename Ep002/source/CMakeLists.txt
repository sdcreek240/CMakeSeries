cmake_minimum_required(VERSION 3.5)
project(HelloApp 
        VERSION 0.0.1
        DESCRIPTION "The leading Hello world app"
        LANGUAGES CXX)

#What do we want to build
add_executable(HelloAppBinary main.cpp)

#Pass special flags to use c++20
target_compile_features(HelloAppBinary PRIVATE cxx_std_20)
