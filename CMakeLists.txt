cmake_minimum_required(VERSION 2.8)
set (CMAKE_CXX_STANDARD 11)
project( DisplayImage )

find_package( OpenCV REQUIRED )
include_directories(${OpenCV_INCLUDE_DIRS})

add_executable( DisplayImage test.cpp )
target_link_libraries( DisplayImage pthread ${OpenCV_LIBS})
