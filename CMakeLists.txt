cmake_minimum_required (VERSION 3.16)

add_library (glad STATIC
        include/glad/glad.h
        include/KHR/khrplatform.h
        src/glad.c
)

set_target_properties (glad
    PROPERTIES
        LINKER_LANGUAGE C
)

target_include_directories (glad PUBLIC include)

