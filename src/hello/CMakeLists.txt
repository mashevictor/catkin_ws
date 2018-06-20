cmake_minimum_required(VERSION 2.8.3)
project(hello)
find_package(catkin REQUIRED COMPONENTS
  roscpp
  rospy
  std_msgs
)
catkin_package(
include_directories(
  ${catkin_INCLUDE_DIRS}
)
add_executable(hello /home/victor/catkin_ws/src/hello/src/hello.cpp)
target_link_libraries(hello ${catkin_LIBRARIES})
