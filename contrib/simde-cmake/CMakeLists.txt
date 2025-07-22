set(SIMDE_LIBRARY_DIR ${ClickHouse_SOURCE_DIR}/contrib/simde)
add_library(_simde INTERFACE)
target_include_directories(_simde SYSTEM INTERFACE ${SIMDE_LIBRARY_DIR}/)
add_library(ch_contrib::simde ALIAS _simde)
