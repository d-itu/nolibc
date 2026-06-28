cmake_minimum_required(VERSION 3.16)

project(nolibc LANGUAGES C)

add_library(nolibc INTERFACE)

target_include_directories(nolibc INTERFACE
  $<BUILD_INTERFACE:${CMAKE_CURRENT_SOURCE_DIR}/include>
  $<INSTALL_INTERFACE:include>
)
