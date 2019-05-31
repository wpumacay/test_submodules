cmake_minimum_required( VERSION 3.0.0 )

project( test_submodules )

set( CMAKE_CXX_STANDARD 11 )
set( CMAKE_CXX_FLAGS "-g ${CMAKE_CXX_FLAGS}" )

add_subdirectory( ext/cat1 )
add_subdirectory( ext/imgui )
add_subdirectory( ext/pybind11 )

add_subdirectory( tysoc )