cmake_minimum_required(VERSION 2.8.3)
project(boxxy_description)

find_package(catkin REQUIRED COMPONENTS
  urdf
)

catkin_package(
#  CATKIN_DEPENDS urdf
)


install(DIRECTORY launch/ DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/launch)
install(DIRECTORY urdf/ DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/urdf)
install(DIRECTORY config/ DESTINATION ${CATKIN_PACKAGE_SHARE_DESTINATION}/config)

