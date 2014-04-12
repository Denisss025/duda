cmake_minimum_required(VERSION 2.8)

set(SRC
	duda.c
	duda_api.c
	duda_body_buffer.c
	duda_conf.c
	duda_console.c
	duda_cookie.c
	duda_data.c
	duda_debug.c
	duda_event.c
	duda_fconf.c
	duda_gc.c
	duda_global.c
	duda_log.c
	duda_map.c
	duda_mem.c
	duda_package.c
	duda_param.c
	duda_qs.c
	duda_queue.c
	duda_request.c
	duda_response.c
	duda_sendfile.c
	duda_session.c
	duda_stats.c
	duda_utils.c
	duda_worker.c
	duda_xtime.c
)

add_library(monkey-duda ${SRC})
