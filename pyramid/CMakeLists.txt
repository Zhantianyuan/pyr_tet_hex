cmake_minimum_required(VERSION 2.8)

PROJECT(Pyramid)

find_package(VTK REQUIRED)
include(${VTK_USE_FILE})

add_executable(Pyramid MACOSX_BUNDLE Pyramid.cxx )

target_link_libraries(Pyramid ${VTK_LIBRARIES})