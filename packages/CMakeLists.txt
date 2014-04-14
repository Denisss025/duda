cmake_minimum_required(VERSION 2.8)

macro(SUBDIRLIST result directory)
	set(listing "")
	file(GLOB children RELATIVE ${directory} ${directory}/*)
	foreach(child ${children})
		if(IS_DIRECTORY ${directory}/${child})
			list(APPEND listing ${child})
		endif()
	endforeach()
	set(${result} ${listing})
endmacro()

SUBDIRLIST(SUBDIRS ${CMAKE_CURRENT_SOURCE_DIR})

foreach(subdir ${SUBDIRS})
	message(STATUS "Package ${subdir} enabled")
	add_subdirectory(${subdir})
endforeach()
