cmake_minimum_required(VERSION 3.4)
project(solver)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
#add_library(formatter_ex STATIC /home/grisha/grigorii05/workspace/tasks/lab03/formatter_ex_lib/formatter_ex.cpp)
#add_library(solver STATIC /home/grisha/grigorii05/workspace/tasks/lab03/solver_lib/solver.cpp)
include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
#add_library(formatter_ex STATIC ${CMAKE_CURRENT_SOURCE_DIR}/formatter_ex.cpp)
#add_library(solver STATIC ${CMAKE_CURRENT_SOURCE_DIR}/solver.cpp)
add_executable(equation ${CMAKE_CURRENT_SOURCE_DIR}/equation.cpp)
target_link_libraries(equation solver)
target_link_libraries(equation formatter_ex)
