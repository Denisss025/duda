cmake_minimum_required(VERSION 2.8)

configure_file(
	"${CMAKE_CURRENT_SOURCE_DIR}/duda.conf.in"
	"${CMAKE_CURRENT_BINARY_DIR}/duda.conf"
)
