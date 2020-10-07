cmake_minimum_required(VERSION 3.5)

project(firstDemo)
set(CMAKE_CXX_STANDARD 14)
find_package(OpenCV REQUIRED)

INCLUDE_DIRECTORIES(${OpenCV_INCLUDE_DIRS})
FILE(GLOB srcs *.cpp)
SET(SRC_LIST ${srcs})

ADD_EXECUTABLE(firstDemo ${SRC_LIST})

TARGET_LINK_LIBRARIES(firstDemo ${OpenCV_LIBS})
