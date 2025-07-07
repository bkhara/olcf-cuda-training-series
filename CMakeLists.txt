cmake_minimum_required(VERSION 3.18)
project(olcf-cuda-training-series LANGUAGES C CXX CUDA)

set(CMAKE_CXX_STANDARD 14)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(CUDA REQUIRED)
find_package(CUDAToolkit REQUIRED)

# Enable CUDA if needed
add_executable(hw1_hello      exercises/hw1/hello.cu)
add_executable(hw1_vector_add exercises/hw1/vector_add.cu)
add_executable(hw1_matrix_mul exercises/hw1/matrix_mul.cu)
