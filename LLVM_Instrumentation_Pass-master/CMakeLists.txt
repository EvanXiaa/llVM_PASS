cmake_minimum_required(VERSION 3.16)
project(LLVM_Instrumentation_Pass_master)

set(CMAKE_CXX_STANDARD 14)

add_executable(LLVM_Instrumentation_Pass_master
        examples/buffer/buffer.c
        examples/performance/main.c
        InstrumentFunctions/logger.c
        InstrumentFunctions/Pass.cpp)
include_directories("/usr/local/Cellar/llvm/11.0.0/include")
