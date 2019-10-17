add_contract(eonio.bios eonio.bios ${CMAKE_CURRENT_SOURCE_DIR}/src/eonio.bios.cpp)

target_include_directories(eonio.bios
   PUBLIC
   ${CMAKE_CURRENT_SOURCE_DIR}/include)

set_target_properties(eonio.bios
   PROPERTIES
   RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_BINARY_DIR}")
