cmake_minimum_required(VERSION 3.2...3.30 FATAL_ERROR)

set(PROJECT_NAME BattleCity)

project(${PROJECT_NAME})

add_executable(BattleCity src/main.cpp)

set(GLFW_INSTALL OFF CACHE BOOL "" FORCE)

add_subdirectory(external/glfw)

target_link_libraries(${PROJECT_NAME} glfw)