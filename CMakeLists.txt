cmake_minimum_required(VERSION 3.10)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(CMAKE_BUILD_TYPE Debug CACHE STRING "Build type" FORCE)

add_executable(main
    # ...
)

target_include_directories(main PRIVATE
    ${CMAKE_CURRENT_SOURCE_DIR}
)

include(CTest)

add_test(NAME run_project COMMAND main)
