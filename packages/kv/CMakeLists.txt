cmake_minimum_required(VERSION 2.8)

set(SRC
	duda_package.c
	unqlite.c
)

add_library(monkey-duda-kv ${SRC})
