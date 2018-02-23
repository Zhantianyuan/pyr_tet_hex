cmake_minimum_required(VERSION 2.8)

PROJECT(Tetrahedron)

find_package(VTK REQUIRED)
include(${VTK_USE_FILE})

add_executable(Tetrahedron MACOSX_BUNDLE Tetrahedron.cxx )

target_link_libraries(Tetrahedron ${VTK_LIBRARIES})