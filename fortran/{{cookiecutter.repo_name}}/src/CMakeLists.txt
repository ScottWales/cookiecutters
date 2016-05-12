set(SOURCES foo.f90)

add_library({{cookiecutter.repo_name}} ${SOURCES})
target_include_directories(hello PUBLIC
    $<BUILD_INTERFACE:${CMAKE_CURRENT_BINARY_DIR}>
    )

add_executable({{cookiecutter.repo_name}}.exe main.f90)
target_link_libraries({{cookiecutter.repo_name}}.exe {{cookiecutter.repo_name}})
set_target_properties({{cookiecutter.repo_name}}.exe PROPERTIES OUTPUT_NAME {{cookiecutter.repo_name}})
