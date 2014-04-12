cmake_minimum_required(VERSION 2.8)

set(SRC
	base64.c
	duda_package.c
)

add_library(monkey-duda-base64 ${SRC})
