cmake_minimum_required(VERSION 3.3)

project(boost_numeric_conversion)

add_library(boost_numeric_conversion INTERFACE)

target_include_directories(boost_numeric_conversion BEFORE INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/include)

install(TARGETS boost_numeric_conversion DESTINATION lib)
install(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/include/boost DESTINATION include)
