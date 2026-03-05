cmake_minimum_required(VERSION 3.0)
project(fftconvolver)

file(GLOB_RECURSE sources      src/*.cpp src/*.h)

add_executable(fftconvolver ${sources})

target_include_directories(fftconvolver PUBLIC src)