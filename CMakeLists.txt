cmake_minimum_required(VERSION 3.10)
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)

project(ImGui)

add_library(${PROJECT_NAME}
    imgui.cpp
    imgui_demo.cpp
    imgui_draw.cpp
    imgui_tables.cpp
    imgui_widgets.cpp

    ./misc/cpp/imgui_stdlib.cpp
)

target_include_directories(${PROJECT_NAME} PUBLIC
    ./
    ./misc/cpp/
)

