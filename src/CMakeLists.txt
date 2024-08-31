# Add executable target with source files
add_executable(LibrealsenseWebcam main.cpp)

# Link with the librealsense libraries as specified during the installation
target_link_libraries(LibrealsenseWebcam PRIVATE realsense2::fw realsense2::rsutils realsense2::realsense2 realsense2::realsense-file)
