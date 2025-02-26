cmake_minimum_required(VERSION 3.29)

project(Laboratorio-Programmazione)

find_package(SFML 2.5 COMPONENTS graphics window system REQUIRED)

include_directories(${SFML_INCLUDE_DIR})

set(SFML_DIR "/opt/homebrew/lib/cmake/SFML/SFMLConfig.cmake/")

add_executable(Laboratorio-Programmazione main.cpp)

set(CMAKE_CXX_STANDARD 20)

target_link_libraries(Laboratorio-Programmazione sfml-graphics sfml-audio)

