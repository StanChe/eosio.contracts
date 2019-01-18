add_contract(vesting.token vesting.token ${CMAKE_CURRENT_SOURCE_DIR}/src/vesting.token.cpp)
target_include_directories(vesting.token.wasm
   PUBLIC
   ${CMAKE_CURRENT_SOURCE_DIR}/include)

set_target_properties(vesting.token.wasm
   PROPERTIES
   RUNTIME_OUTPUT_DIRECTORY "${CMAKE_CURRENT_BINARY_DIR}")
