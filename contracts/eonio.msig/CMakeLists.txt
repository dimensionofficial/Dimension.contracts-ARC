add_contract(eonio.msig eonio.msig ${CMAKE_CURRENT_SOURCE_DIR}/src/eonio.msig.cpp)

target_include_directories(eonio.msig
   PUBLIC
   ${CMAKE_CURRENT_SOURCE_DIR}/include)

set_target_properties(eonio.msig
   PROPERTIES
   RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_BINARY_DIR}")
