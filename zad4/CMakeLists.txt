cmake_minimum_required(VERSION 3.10)
include_directories(include)

project(studProgram)
add_executable(studProgram src/libtest.cpp)
add_library(studlib SHARED src/Student.cpp)
target_link_libraries(studProgram studlib)
install(TARGETS studProgram DESTINATION /usr/bin)
install(TARGETS studlib DESTINATION /usr/lib)
