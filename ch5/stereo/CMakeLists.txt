cmake_minimum_required(VERSION 2.8)

set(CMAKE_BUILD_TYPE "Release")
set(CMAKE_CXX_FLAGS "-std=c++11 -O2")

find_package(OpenCV REQUIRED)
find_package(Pangolin REQUIRED)



add_executable(stereoVision stereoVision.cpp)
target_link_libraries(stereoVision ${OpenCV_LIBS} ${Pangolin_LIBRARIES})