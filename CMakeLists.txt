cmake_minimum_required(VERSION 3.17.1)

project("Home" VERSION 1.1.0)

add_subdirectory("liby")

add_subdirectory("code")

set(LOL "Laugh out loud")
message("${LOL}")
if("${LOL}" STREQUAL "Laugh out loud")
    message("Condition satisfied")
else()
    message("Not satisfied")
endif()
set(myVal 3)
while("${myVal}" LESS 9)
    message("${myVal}")
    math(EXPR myVal "${myVal} + 1")
endwhile()
foreach(idx RANGE 5)
    message(STATUS "yoo ${idx}")
endforeach()
foreach(idx IN ITEMS foo bar far xag)
    message(STATUS "${idx}")
endforeach(idx IN )


# install(TARGETS "${PROJECT_NAME}" DESTINATION bin)
# install(FILES "Main.cpp" DESTINATION src)

include(CPack)
