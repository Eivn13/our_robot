cmake_minimum_required(VERSION 2.8.3)
project(our_robot)
find_package(catkin REQUIRED COMPONENTS ${PACKAGE_DEPENDENCIES})
catkin_package()

install(DIRECTORY launch configuration_files urdf
        DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}
        USE_SOURCE_PERMISSIONS
)
