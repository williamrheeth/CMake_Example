cmake_minimum_required(VERSION 3.28.1)

include_directories(../include/lib)

add_executable(main main.c)

add_library(LIB STATIC ../include/lib/lib.c)

target_link_libraries(main LIB)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_BINARY_DIR}/bin)
