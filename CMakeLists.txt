cmake_minimum_required(VERSION 3.26)
project(untitled1)

set(CMAKE_CXX_STANDARD 17)

add_subdirectory(Student)
add_executable(untitled1 main.cpp)

target_link_libraries(untitled1 Student)

target_include_directories(untitled1 PUBLIC
    "${PROJECT_BINARY_DIR}"
        "${PROJECT_SOURCE_DIR}/Student"
)