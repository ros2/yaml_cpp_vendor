cmake_minimum_required(VERSION 3.10)
project(yaml_cpp_vendor CXX)

find_package(ament_cmake REQUIRED)
find_package(ament_cmake_vendor_package REQUIRED)

install(DIRECTORY cmake
  DESTINATION share/${PROJECT_NAME})

ament_package(
  CONFIG_EXTRAS "yaml_cpp_vendor-extras.cmake"
)
