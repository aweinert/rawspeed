add_executable(rsbench main.cpp)
set_target_properties(rsbench PROPERTIES LINKER_LANGUAGE CXX)
target_link_libraries(rsbench rawspeed_benchmark)
target_include_directories(rsbench PUBLIC "${CONFIG_INCLUDE_PATH}")
add_dependencies(benchmarks rsbench)
