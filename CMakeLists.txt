################################################################################
# CMakeLists.txt - root CMake configuration file, part PostGIS project
#
# Copyright (C) 2020, NextGIS <info@nextgis.com>
################################################################################
cmake_minimum_required (VERSION 2.8.12 FATAL_ERROR)
project(postgis NONE)

set(VERSION_FILE ${CMAKE_CURRENT_SOURCE_DIR}/CMakeLists.txt)
set(VERSION 2.5.8)
file(TIMESTAMP ${VERSION_FILE} VERSION_DATETIME "%Y-%m-%d %H:%M:%S" UTC)
file(WRITE ${CMAKE_BINARY_DIR}/version.str "${VERSION}\n${VERSION_DATETIME}")
