cmake_minimum_required(VERSION 3.7)
project(TinyCompiler)

set(CMAKE_CXX_STANDARD 11)

set(SOURCE_FILES
        ASTNodes.h
        CodeGen.h
        grammar.cpp
        grammar.hpp
        grammar.y
        main.cpp
        Makefile
        test.input
        token.cpp
        token.l CodeGen.cpp utils.cpp ObjGen.cpp ObjGen.h TypeSystem.h TypeSystem.cpp Types.h)

add_executable(TinyCompiler ${SOURCE_FILES})