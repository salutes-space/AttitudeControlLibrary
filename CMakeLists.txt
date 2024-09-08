cmake_minimum_required (VERSION 3.15)

project(AttitudeMathLib)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED True)

add_subdirectory(AML)
add_subdirectory(example)
add_subdirectory(test)

enable_testing()
add_test(test_all test/AML_Test)
