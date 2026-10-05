add_executable(hello-window "${CMAKE_CURRENT_SOURCE_DIR}/main.cpp")

target_link_libraries(hello-window 
    PRIVATE
        glad
        glfw
        gld
)