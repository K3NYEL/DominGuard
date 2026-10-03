cmake_minimum_required(version 3.21)

project(
    VERSION 0.1.0
    LANGUAGEs CXX
)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_AUTORCC ON)

find_package(
    Core
    Gui
    Widgets
)

add_executable(
    src/main.cpp
)

target_link_libraries(
    PRIVATE
        Qt6: Core 
        Qt6: Gui
        Qt6: Widgets  
)