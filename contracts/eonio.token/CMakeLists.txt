add_contract(eonio.token eonio.token ${CMAKE_CURRENT_SOURCE_DIR}/src/eonio.token.cpp)

target_include_directories(eonio.token
   PUBLIC
   ${CMAKE_CURRENT_SOURCE_DIR}/include)

set_target_properties(eonio.token
   PROPERTIES
   RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_BINARY_DIR}")
