cmake_minimum_required(VERSION 3.17.1)

project("Home" VERSION 1.1.0)

add_subdirectory("liby")

add_subdirectory("code")

# install(TARGETS "${PROJECT_NAME}" DESTINATION bin)
# install(FILES "Main.cpp" DESTINATION src)

include(CPack)
