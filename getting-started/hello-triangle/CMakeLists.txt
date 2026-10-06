add_executable(hello-triangle "${CMAKE_CURRENT_SOURCE_DIR}/main.cpp")

target_link_libraries(hello-triangle 
    PRIVATE
        glad
        glfw
        gld
)