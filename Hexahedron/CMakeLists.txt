cmake_minimum_required(VERSION 2.8)

PROJECT(Hexahedron)

find_package(VTK REQUIRED)
include(${VTK_USE_FILE})

add_executable(Hexahedron MACOSX_BUNDLE Hexahedron.cxx )

target_link_libraries(Hexahedron ${VTK_LIBRARIES})
