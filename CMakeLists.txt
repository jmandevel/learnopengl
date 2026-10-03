cmake_minimum_required(VERSION 4.3.2)

project(learnopengl)

add_executable(learnopengl "")

add_subdirectory(src)

target_include_directories(learnopengl
    PRIVATE
        "${CMAKE_CURRENT_SOURCE_DIR}/include"
)

Include(FetchContent)
FetchContent_Declare(glfw
    GIT_REPOSITORY https://github.com/glfw/glfw
    GIT_TAG        3.5.1
)
FetchContent_MakeAvailable(glfw)

Include(FetchContent)
FetchContent_Declare(glm
    GIT_REPOSITORY https://github.com/g-truc/glm
    GIT_TAG        1.0.3
)
FetchContent_MakeAvailable(glm)

Include(FetchContent)
FetchContent_Declare(assimp
    GIT_REPOSITORY https://github.com/assimp/assimp
    GIT_TAG        v6.0.5
)
FetchContent_MakeAvailable(assimp)

Include(FetchContent)
FetchContent_Declare(gld
    GIT_REPOSITORY https://github.com/jmandevel/gld.h
    GIT_TAG        2.0.0.0
)
FetchContent_MakeAvailable(gld)

target_link_libraries(learnopengl
    PRIVATE
        glfw
        glm
        assimp
        gld
)