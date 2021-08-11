cmake_minimum_required(VERSION 3.17)

project(PicoSHA2 LANGUAGES CXX)

include(GNUInstallDirs)


add_library(PicoSHA2 INTERFACE)
target_sources(PicoSHA2 INTERFACE picosha2.h)

install(FILES picosha2.h DESTINATION ${CMAKE_INSTALL_INCLUDEDIR})
