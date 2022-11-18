# cmake version to be used
cmake_minimum_required(VERSION 3.0)

# project name
project(point_cloud_merger)

set (CMAKE_CXX_STANDARD 17)

find_package(PCL 1.3 REQUIRED)

include_directories(${PCL_INCLUDE_DIRS} "include")
link_directories(${PCL_LIBRARY_DIRS})
add_definitions(${PCL_DEFINITIONS})

set(CMAKE_CXX_FLAGS "-Wall -Wextra -O3")

# target
add_executable(main  ./src/main.cpp)

target_link_libraries(main ${PCL_LIBRARIES} "stdc++fs")
