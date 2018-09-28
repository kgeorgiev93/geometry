cmake_minimum_required(VERSION 2.8.3)

include(cmake/HunterGate.cmake)
HunterGate(
    URL "https://github.com/ruslo/hunter/archive/v0.23.212.tar.gz"
    SHA1 "4aa1b334bd73f7409beac209296e6e5c7758df21"
)

project(geometry)

hunter_add_package(angles)
hunter_add_package(ros_common_msgs)
hunter_add_package(ros_message_generation)
hunter_add_package(ros_comm)
hunter_add_package(ros_std_msgs)
hunter_add_package(tf2)

add_subdirectory(tf)

# Omitted, have orocos-kdl as dependency
#add_subdirectory(eigen_conversions)
#add_subdirectory(kdl_conversions)
#add_subdirectory(tf_conversions)
