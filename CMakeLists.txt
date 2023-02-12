cmake_minimum_required(VERSION 3.20)

project(eigen)

set(CMAKE_CXX_STANDARD 17)

add_library(${PROJECT_NAME} INTERFACE)
target_include_directories(
  ${PROJECT_NAME}
  INTERFACE ${CMAKE_CURRENT_SOURCE_DIR} ${CMAKE_CURRENT_SOURCE_DIR}/Eigen
            ${CMAKE_CURRENT_SOURCE_DIR}/Eigen/src)
