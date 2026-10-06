add_executable(vertex-out "${CMAKE_CURRENT_SOURCE_DIR}/main.cpp")

target_link_libraries(vertex-out 
    PRIVATE
        glad
        glfw
        gld
)