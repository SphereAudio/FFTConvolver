cmake_minimum_required(VERSION 3.5)
project(fftconvolver)

set(LIBRARY_SOURCE
    src/AudioFFT.cpp
    src/AudioFFT.h
    src/FFTConvolver.cpp
    src/FFTConvolver.h
    src/TwoStageFFTConvolver.cpp
    src/TwoStageFFTConvolver.h
    src/Utilities.cpp
    src/Utilities.h
)

add_library(fftconvolver ${LIBRARY_SOURCE})