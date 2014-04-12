cmake_minimum_required(VERSION 2.8)

set(SRC
	base64.c
	broadcast.c
	callbacks.c
	duda_package.c
	request.c
	sha1.c
	websocket.c
)

add_library(monkey-duda-websocket ${SRC})
