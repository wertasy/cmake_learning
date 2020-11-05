add_library(dbs)

add_subdirectory(common)
add_subdirectory(core)

target_link_libraries(dbs
  PUBLIC
    common
    core
  )