cmake_minimum_required(VERSION 3.20)

if (NOT TARGET corosys)
    add_library(corosys INTERFACE)
    target_sources(corosys INTERFACE
        corosys.cpp
    )
    target_include_directories(corosys INTERFACE
        .
    )
endif()
