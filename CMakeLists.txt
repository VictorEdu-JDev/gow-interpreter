cmake_minimum_required(VERSION 3.10)
project(gow_interpreter C)

set(CMAKE_C_STANDARD 99)

include_directories(interfaces)

add_executable(gowc main.c
        src/interpreter.c
        src/lexer.c
        src/parser.c
        src/ast.c
        interfaces/ast.h
        src/symbol_table.c
        interfaces/symbol_table.h
)
