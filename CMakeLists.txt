cmake_minimum_required(VERSION 3.9)
project(bfx_cpp_api)

set(CMAKE_CXX_STANDARD 11)

add_executable(bfx_cpp_api
        BitfinexAPI.cpp
        BitfinexAPI.hpp
        example.cpp
        withdraw.conf)
target_link_libraries(bfx_cpp_api -lcryptopp -lcurl)