add_executable(hello-square "${CMAKE_CURRENT_SOURCE_DIR}/main.cpp")

target_link_libraries(hello-square 
    PRIVATE
        glad
        glfw
        gld
)