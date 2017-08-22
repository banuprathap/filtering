PROJECT(Filters)

CMAKE_MINIMUM_REQUIRED(VERSION 3.2.1)

include(CMakeToolsHelpers OPTIONAL)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_CXX_FLAGS "-Wall -Wextra -Wpedantic")
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF) ## on g++ this ensures: -std=c++11 and not -std=gnu++11

#############################################################################
# Add subdirectories in the PROJECT
#############################################################################

add_subdirectory(src)
add_subdirectory(test)
add_subdirectory(vendor/googletest/googletest)

###############################################################################