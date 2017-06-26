cmake_minimum_required(VERSION 3.7)
project(denseTrajectories)
FIND_PACKAGE(OpenCV REQUIRED)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES DenseTrack.cpp)
add_executable(denseTrajectories ${SOURCE_FILES})
target_link_libraries(denseTrajectories ${OpenCV_LIBS})