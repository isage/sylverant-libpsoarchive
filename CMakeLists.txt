cmake_minimum_required( VERSION 2.8 )

project( libpsoarchive )

set(libpsoarchive_MAJOR_VERSION "1")
set(libpsoarchive_MINOR_VERSION "0")


file(GLOB SOURCES src/*.c)

add_definitions (-Wall)
include_directories(${CMAKE_SOURCE_DIR}/include)

add_library(psoarchive STATIC ${SOURCES})
