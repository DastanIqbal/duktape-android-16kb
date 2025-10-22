cmake_minimum_required(VERSION 3.10)

# Project declaration
project(duktape)

file(GLOB_RECURSE duktape_SRC
    "*.c"
    "*.cpp"
)

add_library(duktape SHARED ${duktape_SRC})

target_link_libraries(duktape)
