#cplusplus project top CmakeLists
#author : Liqiang Yang
#e-mail : tongchi216@163.com
#date   : 2021-1-28
cmake_minimum_required(VERSION 3.5)

project(cplusplus)

set(CMAKE_INSTALL_PREFIX ${PROJECT_SOURCE_DIR}/install)
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/install/bin)
set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/install/lib)
set(CMAKE_INSTALL_INCLUDEDIR ${PROJECT_SOURCE_DIR}/install/include)
set(INCLUDE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/install/include)
include_directories(SYSTEM ${PROJECT_SOURCE_DIR}/install/include)
link_directories(${LIBRARY_OUTPUT_PATH})

add_subdirectory(normal_demo)
add_subdirectory(socket_demo)

