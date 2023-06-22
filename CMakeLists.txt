cmake_minimum_required(VERSION 3.7)

project (PROJECT_NAME)

set (CMAKE_CXX_STANDARD 17)
set (CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

file(GLOB PROJECT_SRC CONFIGURE_DEPENDS "include/**.h" "include/**.cpp" "src/**.h" "src/**.cpp")

add_executable(PROJECT_NAME ${PROJECT_SRC})
