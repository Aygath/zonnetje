configure_file(ZonnetjeConfig.h.in ZonnetjeConfig.h)
add_executable(zonnetje zon.c)
target_link_libraries(zonnetje m)

