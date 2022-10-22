cmake_minimum_required(VERSION 3.10.2)
project(cmake_learn)

set(CMAKE_CXX_STANDARD 14)

add_subdirectory(src bin)

install(FILES LICENSE README.md DESTINATION share/doc/cmake/)
install(PROGRAMS run.sh DESTINATION bin)
install(DIRECTORY doc/ DESTINATION share/doc/cmake)



