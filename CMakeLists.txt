cmake_minimum_required(VERSION 3.1)
project(my-project VERSION 1.0)

# Handling compile_command.json
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)
add_custom_target(link_target ALL
  COMMAND ${CMAKE_COMMAND} -E create_symlink ${CMAKE_BINARY_DIR}/compile_commands.json ${CMAKE_SOURCE_DIR}/compile_commands.json)

# actual source code
add_subdirectory(src)
