cmake_minimum_required(VERSION 2.8)
project(libexpat CXX)

###############
# ASI default settings
list(APPEND CMAKE_MODULE_PATH "$ENV{ASV_CMAKE}")
include(asv_cmake_defaults)
asv_cmake_defaults( )
###############

# sweet shared code..
set(EXPAT_SHARED_LIBS ON)

set(EXPAT_BUILD_TOOLS OFF)
set(EXPAT_BUILD_EXAMPLES OFF)
set(EXPAT_BUILD_TESTS OFF)
set(EXPAT_BUILD_DOCS OFF)
set(EXPAT_ENABLE_INSTALL ON)

add_subdirectory(expat)
