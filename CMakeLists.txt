cmake_minimum_required (VERSION 2.8)

# projectname is the same as the main-executable
project(mini_factor)

#add_definitions('-g')
#add_definitions('-Wall')
add_definitions('-std=c++11')

add_executable(${PROJECT_NAME} mini_factor.cpp)
