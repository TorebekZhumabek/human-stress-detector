cmake_minimum_required(VERSION 2.8)
project( path-detector )
find_package( OpenCV REQUIRED )
add_executable( detectpeople detectpeople.cpp )
set(EXECUTABLE_OUTPUT_PATH ${CMAKE_BINARY_DIR}/bin)
target_link_libraries( detectpeople ${OpenCV_LIBS} )