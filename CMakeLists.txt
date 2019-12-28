cmake_minimum_required (VERSION 2.8)

project(mini_factor)

add_definitions('-std=c++11')

add_executable(${PROJECT_NAME} mini_factor.cpp)

include(CTest)
enable_testing()

file(GLOB t "${CMAKE_CURRENT_SOURCE_DIR}/t/*.t")
add_test(
    NAME prove
    COMMAND prove ${t}
)
