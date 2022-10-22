cmake_minimum_required(VERSION 3.10.2)
project(cmake_learn)

set(CMAKE_CXX_STANDARD 14)

set(SRC_LIST src/main.cpp)

add_subdirectory(lib)

add_executable(${PROJECT_NAME} ${SRC_LIST})

target_link_libraries(${PROJECT_NAME} PUBLIC hello)
target_include_directories(${PROJECT_NAME} PUBLIC ${PROJECT_SOURCE_DIR}/lib)





