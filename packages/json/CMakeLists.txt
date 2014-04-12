cmake_minimum_required(VERSION 2.8)

set(SRC
	cJSON.c
	duda_package.c
)

add_library(monkey-duda-json ${SRC})
