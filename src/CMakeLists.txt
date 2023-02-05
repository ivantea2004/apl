


file(GLOB_RECURSE headers ${APL_ROOT}/include/apl/*.hpp)

add_library(apl INTERFACE ${headers})

target_compile_features(apl INTERFACE cxx_std_20)

target_include_directories(apl INTERFACE ${APL_ROOT}/include)

add_library(apl::apl ALIAS apl)


