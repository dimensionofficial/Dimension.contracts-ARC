add_contract(eonio.wrap eonio.wrap ${CMAKE_CURRENT_SOURCE_DIR}/src/eonio.wrap.cpp)

target_include_directories(eonio.wrap
   PUBLIC
   ${CMAKE_CURRENT_SOURCE_DIR}/include)

set_target_properties(eonio.wrap
   PROPERTIES
   RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_BINARY_DIR}")
