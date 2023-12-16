# CMakeLists.txt

cmake_minimum_required(VERSION 3.10)

project(sfml-app)

# Find SFML
find_package(SFML 2.5 COMPONENTS graphics window system REQUIRED)

# Set C++ standard to 17
set(CMAKE_CXX_STANDARD 17)

# Include directories
include_directories(${SFML_INCLUDE_DIR})

# Set the output directory for build artifacts
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)

# Source files
file(GLOB_RECURSE SOURCES "src/*.cpp")

# Executable
add_executable(sfml-app ${SOURCES})

# Link SFML libraries
target_link_libraries(sfml-app PRIVATE sfml-graphics sfml-window sfml-system)
