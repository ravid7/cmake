add_library("tester" 
    SHARED
    "${CMAKE_CURRENT_SOURCE_DIR}/src/Hello.hpp"
    "${CMAKE_CURRENT_SOURCE_DIR}/src/Hello.cpp"
    )

target_include_directories("tester" PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/src")