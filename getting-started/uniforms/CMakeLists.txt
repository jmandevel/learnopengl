add_executable(uniforms "${CMAKE_CURRENT_SOURCE_DIR}/main.cpp")

target_link_libraries(uniforms 
    PRIVATE
        glad
        glfw
        gld
)