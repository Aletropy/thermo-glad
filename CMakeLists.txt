cmake_minimum_required(VERSION 3.1...3.29)

project(ThermoGlad LANGUAGES C)

add_library(ThermoGlad STATIC
        src/glad.c

        include/glad/glad.h
        include/KHR/khrplatform.h
)

target_include_directories(ThermoGlad PUBLIC include)