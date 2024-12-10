cmake_minimum_required(VERSION 3.10)
project(curiosity)
set(CMAKE_CXX_STANDARD 17)

# colorful message
string(ASCII 27 ESC)
set(BOLD_RED "${ESC}[1;31m")
set(BOLD_GREEN "${ESC}[1;32m")
set(BOLD_YELLOW "${ESC}[1;33m")
set(BOLD_MAGENTA "${ESC}[1;35m")
set(BOLD_CYAN "${ESC}[1;36m")
set(CLR "${ESC}[m")

# add support for vscode clangd plugin
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/rsg_envs/bin)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/rsg_envs/libs)
set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR}/rsg_envs/libs)
set(CMAKE_POLICY_DEFAULT_CMP0148 NEW)
set(CMAKE_POLICY_DEFAULT_CMP0077 NEW)

# set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fopenmp -march=native")
# set(CMAKE_CXX_FLAGS_DEBUG "-O0 -ggdb")
# set(CMAKE_CXX_FLAGS_RELEASE "-fPIC -Ofast -flto=auto -DEIGEN_NO_DEBUG")
