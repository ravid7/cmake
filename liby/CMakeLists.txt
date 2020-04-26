add_library("tester" 
    "${CMAKE_CURRENT_SOURCE_DIR}/src/internal/Hello.hpp"
    "${CMAKE_CURRENT_SOURCE_DIR}/src/internal/Hello.cpp"
    )

target_include_directories("tester" PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/src/internal")

target_compile_definitions("tester" INTERFACE RAVI_RATHORE=42)