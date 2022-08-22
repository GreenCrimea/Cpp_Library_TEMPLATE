cmake_minimum_required(VERSION 3.0.0)
project(cpp_library_test VERSION 0.1.0)


INCLUDE_DIRECTORIES(
    /home/gc/vcpkg/installed/x64-linux/include/cryptopp
)

LINK_DIRECTORIES(
    /home/gc/vcpkg/installed/x64-linux/lib
)


add_executable(cpp_library_test main.cpp)


TARGET_LINK_LIBRARIES(cpp_library_test
    cryptopp
)