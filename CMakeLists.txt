# CMakeLists files in this project can
# refer to the root source directory of the project as ${HELLO_SOURCE_DIR} and
# to the root binary directory of the project as ${HELLO_BINARY_DIR}.
cmake_minimum_required (VERSION 2.8.7)
project (UTEST)

add_executable(factorial test.cpp)
add_executable(mine test2.cpp)

enable_testing()
add_test (factorial factorial)
add_test (mine mine)
