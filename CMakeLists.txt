cmake_minimum_required(VERSION 2.8.3)

include(cmake/HunterGate.cmake)
HunterGate(
  URL "https://github.com/lsolanka/hunter/archive/v0.22.4-rosdevel15.tar.gz"
  SHA1 "40d2da7c46f9cb5efc78396f90c9b00a7c73b21a"
)

project(geometry)

add_subdirectory(tf)
