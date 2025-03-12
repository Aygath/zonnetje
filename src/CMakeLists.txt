configure_file(ZonnetjeConfig.h.in ZonnetjeConfig.h)

set (CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR})
add_executable(zonnetje zon.c)
target_include_directories(zonnetje PRIVATE ${PROJECT_BINARY_DIR}/src)
target_link_libraries(zonnetje m)

