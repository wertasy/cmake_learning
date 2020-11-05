add_library(core OBJECT)

aux_source_directory(${CMAKE_CURRENT_LIST_DIR}/source CORE_SOURCES)

target_sources(core
  PRIVATE
      ${CORE_SOURCES}
  )

target_include_directories(core
  PUBLIC
      ${CMAKE_CURRENT_LIST_DIR}/include
  PRIVATE
      ${CMAKE_CURRENT_LIST_DIR}/../common/include
  )