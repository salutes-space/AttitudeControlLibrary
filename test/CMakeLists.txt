cmake_minimum_required (VERSION 3.15)

project(AML_Test)

add_executable(${PROJECT_NAME} 
               main.cpp
               AMLVector3Test.cpp
               AMLMatrix33Test.cpp
               AMLDCMTest.cpp
               )

target_link_libraries(
    ${PROJECT_NAME}
    AML
)

install(TARGETS ${PROJECT_NAME}
    DESTINATION ${CMAKE_BINARY_DIR}/bin
)