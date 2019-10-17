cmake_minimum_required( VERSION 3.5 )

project(contracts)

set(EOSIO_WASM_OLD_BEHAVIOR "Off")
find_package(eosio.cdt)

add_subdirectory(eonio.bios)
add_subdirectory(eonio.msig)
add_subdirectory(eonio.system)
add_subdirectory(eonio.token)
add_subdirectory(eonio.wrap)
