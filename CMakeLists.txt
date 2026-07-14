cmake_minimum_required(VERSION 3.20)

project(OOP_Bank_Management_System LANGUAGES CXX)

if(NOT MSVC)
    message(FATAL_ERROR
        "This project uses Microsoft C++ extensions such as __declspec(property). "
        "Configure it with the Visual Studio 2022 MSVC toolchain."
    )
endif()

add_executable(OOP_Bank_Management_System main.cpp)

target_compile_features(OOP_Bank_Management_System PRIVATE cxx_std_17)
target_compile_options(OOP_Bank_Management_System PRIVATE
    /permissive-
    /Zc:__cplusplus
)

set_property(TARGET OOP_Bank_Management_System PROPERTY
    VS_DEBUGGER_WORKING_DIRECTORY "${CMAKE_SOURCE_DIR}/Data"
)
