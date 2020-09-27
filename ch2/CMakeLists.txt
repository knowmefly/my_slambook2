# define version
cmake_minimum_required(VERSION 2.8)

# define project name
project( HelloSLAM )

# add exe project
#add_executable(helloSLAM helloSLAM.cpp)

add_library(hello libHelloSLAM.cpp)
add_executable(useHello useHello.cpp)
target_link_libraries(useHello hello)
