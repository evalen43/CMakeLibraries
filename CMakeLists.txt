cmake_minimum_required(VERSION "3.18.1")

#Set target output directory
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
set(CMAKE_LIBRARY_DIRECTORY "${CMAKE_BINARY_DIR}/lib")
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/bin")

option(BUILD_SHARED_LIBS "True when building a shared library" True)


project("Matrix")

add_subdirectory("matrix")

add_subdirectory("examples")