include_directories(${CMAKE_CURRENT_SOURCE_DIR}/pybind11)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/pybind11/include)

set_global_variable (DEPS_INCL_DIR 
    ${CMAKE_CURRENT_SOURCE_DIR}/pybind11
    ${CMAKE_CURRENT_SOURCE_DIR}/pybind11/include
)

set(PYBIND11_CPP_STANDARD -std=c++14)
add_subdirectory(pybind11)
add_subdirectory(libuv)
