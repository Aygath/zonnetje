configure_file(ZonnetjeConfig.h.in ZonnetjeConfig.h)

# Place the executable into the build directory:
set (CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})

add_executable(zonnetje zon.c)
target_link_libraries(zonnetje m)

# Make sure that in case of out-of-source builds, the generated config.h can be found relative to build directory:
target_include_directories(zonnetje PRIVATE ${PROJECT_BINARY_DIR}/src)


