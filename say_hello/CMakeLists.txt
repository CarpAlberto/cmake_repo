add_library (
    say_hello
    src/say_hello/hello.h
    src/say_hello/hello.cpp
)

target_include_directories(say_hello PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/src")

target_compile_definitions(say_hello PUBLIC SAY_HELLO_VERSION=4)