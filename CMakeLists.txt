cmake_minimum_required(VERSION 3.12)

project(FreeGLUT_DEMO)

set(FREEGLUT_BUILD_DEMOS OFF)
set(FREEGLUT_BUILD_SHARED_LIBS ON)
set(FREEGLUT_BUILD_STATIC_LIBS ON)
add_subdirectory(external/FreeGLUT/freeglut/freeglut)


set(BUILD_UTILS OFF)
add_subdirectory(external/glew/build/cmake)

add_executable(smooth_opengl3 smooth_opengl3.c)
