cmake_minimum_required(VERSION 2.8.3)

project(kuka_lwr4_resources_armhf)

find_package(catkin REQUIRED)

catkin_package()

foreach(dir urdf)
  install(DIRECTORY ${dir}/
    DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/${dir})
endforeach()