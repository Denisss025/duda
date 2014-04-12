cmake_minimum_required(VERSION 2.8)

set(SRC
	duda_package.c
	sha1.c
)

add_library(monkey-duda-sha1 ${SRC})
