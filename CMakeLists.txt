cmake_minimum_required(VERSION 3.16)
project(fftconvolver)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

add_library(${PROJECT_NAME} "")

target_sources(${PROJECT_NAME} PRIVATE
    src/AudioFFT.cpp
    src/AudioFFT.h
    src/FFTConvolver.cpp
    src/FFTConvolver.h
    src/TwoStageFFTConvolver.cpp
    src/TwoStageFFTConvolver.h
    src/Utilities.cpp
    src/Utilities.h
)

target_include_directories(${PROJECT_NAME} PUBLIC ${CMAKE_CURRENT_LIST_DIR})