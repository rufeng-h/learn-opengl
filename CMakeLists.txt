cmake_minimum_required(VERSION 3.23)
project(OpenGL)

set(CMAKE_CXX_STANDARD 11)

add_executable(OpenGL src/glad.c main.cpp)

include_directories(include)
link_directories(lib)
target_link_libraries(OpenGL ${PROJECT_SOURCE_DIR}/lib/glfw3.dll)