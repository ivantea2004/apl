
project(example_1)

add_executable(example_1 main.cpp)

target_link_libraries(example_1 PUBLIC apl::apl)

target_compile_features(example_1 PUBLIC cxx_std_20)
