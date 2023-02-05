cmake_minimum_required(VERSION 3.20)

set_property(GLOBAL PROPERTY USE_FOLDERS ON)

project(apl)


set(APL_ROOT ${CMAKE_CURRENT_SOURCE_DIR})

add_subdirectory(${APL_ROOT}/src)

add_subdirectory(${APL_ROOT}/examples)

set_target_properties(apl PROPERTIES FOLDER apl)
set_target_properties(example_1 PROPERTIES FOLDER examples)
