cmake_minimum_required(VERSION 3.10)
project(LibrealsenseWebcam)

# Set C++17 as the standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Specify the MSYS2 path used during the librealsense installation
set(CMAKE_PREFIX_PATH "C:/Users/lab20/Documents/Development/vcpkg/installed/x64-windows")

# Find the librealsense2 package using the configurations from the installation
find_package(realsense2 CONFIG REQUIRED)

include_directories(include)

# Add the source directory
add_subdirectory(src)

# Optionally enable testing and add the tests directory
# enable_testing()
# add_subdirectory(tests)
