cmake_minimum_required(VERSION 3.17)

project(h5pixels)

##
## version
##
set(h5pixels_VERSION_MAJOR 0)
set(h5pixels_VERSION_MINOR 1)

##
## setup the build output structure
##
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

set(CMAKE_CXX_STANDARD 17)
find_package(HDF5 COMPONENTS CXX REQUIRED)

add_subdirectory(src)
