cmake_minimum_required(VERSION 3.4 FATAL_ERROR)

find_package(Qt5 COMPONENTS Quick REQUIRED)
file(GLOB SOURCES *.cpp)
add_library(duperagent ${SOURCES})
target_include_directories(duperagent PUBLIC ${CMAKE_CURRENT_SOURCE_DIR})
target_link_libraries(duperagent Qt::Quick)
