cmake_minimum_required(VERSION 3.22)
project(kokkos-cuda)

add_executable(kokkos-cuda main.cpp)
find_package(Kokkos REQUIRED)
target_link_libraries(kokkos-cuda Kokkos::kokkos)
target_compile_options(kokkos-cuda PRIVATE -DLARGE)
