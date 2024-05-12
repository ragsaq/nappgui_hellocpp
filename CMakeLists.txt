cmake_minimum_required(VERSION 3.0)

project(hellocpp LANGUAGES CXX)

find_package(nappgui REQUIRED)

add_executable(${PROJECT_NAME} WIN32 main.cpp)

target_include_directories(${PROJECT_NAME} PRIVATE ${NAPPGUI_INCLUDES})
target_link_libraries(${PROJECT_NAME} PRIVATE ${NAPPGUI_LIBRARIES})
