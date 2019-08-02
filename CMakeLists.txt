cmake_minimum_required(VERSION 3.10)

project(minimalmilk)

set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake/")
set(OpenGL_GL_PREFERENCE "GLVND")

find_package(SDL2 REQUIRED)
include_directories(${SDL2_INCLUDE_DIRS})

find_package(SDL2_image REQUIRED)
include_directories(${SDL2_IMAGE_DIRS})

find_package(OpenGL REQUIRED)
include_directories(${OPENGL_INCLUDE_DIRS})

find_package(GLEW REQUIRED)
include_directories(${GLEW_INCLUDE_DIRS})

add_executable(minimalmilk WIN32 main.cpp)
target_link_libraries(minimalmilk ${SDL2_LIBRARIES} ${SDL2_IMAGE_LIBRARIES} ${GLEW_LIBRARIES} ${OPENGL_LIBRARIES})
