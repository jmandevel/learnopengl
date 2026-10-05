add_library(glad STATIC "")

add_subdirectory(src)

target_include_directories(glad
    PUBLIC
        "${CMAKE_CURRENT_SOURCE_DIR}/include"
)