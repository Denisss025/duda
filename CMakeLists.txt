cmake_minimum_required(VERSION 2.8)

include_directories(${CMAKE_CURRENT_SOURCE_DIR}/src)

add_subdirectory(conf)
add_subdirectory(src)
add_subdirectory(packages)
add_subdirectory(examples)

file(
	COPY "${CMAKE_CURRENT_SOURCE_DIR}/htdocs"
	DESTINATION "${CMAKE_CURRENT_BINARY_DIR}"
)

