#==============================
# Requirements
#==============================

cmake_minimum_required(VERSION 3.10)

#==============================
# Project Settings
#==============================

if (NOT PROJECT_DECLARED)
    project("Gaia Exceptions" LANGUAGES CXX VERSION 0.9.0)
    set(PROJECT_DECLARED)
endif()

#==============================
# Project Modules
#==============================

add_subdirectory("GaiaExceptions")

if (WITH_TEST)
    add_subdirectory("UnitTest")
endif()
