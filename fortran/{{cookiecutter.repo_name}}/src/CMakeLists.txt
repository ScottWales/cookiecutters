set(SOURCES {{cookiecutter.lib_name}}.f90)

add_library({{cookiecutter.lib_name}} ${SOURCES})
target_include_directories({{cookiecutter.lib_name}} PUBLIC
    $<BUILD_INTERFACE:${CMAKE_CURRENT_BINARY_DIR}>
    $<INSTALL_INTERFACE:include>
    )

add_executable({{cookiecutter.repo_name}}.exe main.f90)
target_link_libraries({{cookiecutter.repo_name}}.exe {{cookiecutter.lib_name}})
set_target_properties({{cookiecutter.repo_name}}.exe PROPERTIES OUTPUT_NAME {{cookiecutter.repo_name}})

install(TARGETS {{cookiecutter.lib_name}} {{cookiecutter.lib_name}}.exe
    RUNTIME DESTINATION bin
    LIBRARY DESTINATION lib
    ARCHIVE DESTINATION lib
    )

install(DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/ DESTINATION include
    FILES_MATCHING PATTERN "*.mod"
    PATTERN "CMakeFiles" EXCLUDE
    )
