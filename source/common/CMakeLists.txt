add_library(common OBJECT)

aux_source_directory(${CMAKE_CURRENT_LIST_DIR}/source COMMON_SOURCES)

target_sources(common
  PRIVATE
      ${COMMON_SOURCES}
  )

target_include_directories(common
  PUBLIC
      ${CMAKE_CURRENT_LIST_DIR}/include
  )