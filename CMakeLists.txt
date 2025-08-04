cmake_minimum_required(VERSION 3.10)

project(genInvertibleMat LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)

set(SRC_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)
set(SRC_FILES
    ${SRC_DIR}/genInvertibleMat.cc
)

add_executable(genInvertibleMat ${SRC_FILES})

set(CMAKE_INSTALL_PREFIX ${CMAKE_CURRENT_SOURCE_DIR})

install(TARGETS genInvertibleMat
    RUNTIME DESTINATION ${CMAKE_INSTALL_PREFIX}/install
)