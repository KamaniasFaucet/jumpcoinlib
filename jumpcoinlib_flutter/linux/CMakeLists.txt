# The Flutter tooling requires that developers have CMake 3.10 or later
# installed. You should not increase this version, as doing so will cause
# the plugin to fail to compile for some customers of the plugin.
cmake_minimum_required(VERSION 3.10)

# Project-level configuration.
set(PROJECT_NAME "jumpcoinlib_flutter")
project(${PROJECT_NAME} LANGUAGES C)

# Invoke the build for native code shared with the other target platforms.
# This can be changed to accomodate different builds.
add_subdirectory("${CMAKE_CURRENT_SOURCE_DIR}/../src" "${CMAKE_CURRENT_BINARY_DIR}/shared")

# List of absolute paths to libraries that should be bundled with the plugin.
# This list could contain prebuilt libraries, or libraries created by an
# external build triggered from this build file.

set(jumpcoinlib_flutter_bundled_libraries
  # Defined in ../src/CMakeLists.txt.
  # This can be changed to accomodate different builds.
  ${CMAKE_BINARY_DIR}/secp256k1/lib/libsecp256k1.so
  PARENT_SCOPE
)
