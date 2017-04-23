project(FoundationTimer)
cmake_minimum_required(VERSION 2.8.12)

include(${CMAKE_BINARY_DIR}/conanbuildinfo.cmake)
conan_basic_setup()

set ( PROJECT_LINK_LIBS libStudent.a )

add_executable(example example.cpp)
target_link_libraries(example ${PROJECT_LINK_LIBS} )
