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
# install(TARGETS "${PROJECT_NAME}" DESTINATION bin)
# install(FILES "Main.cpp" DESTINATION src)

include(CPack)
