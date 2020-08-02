set(FILES "${CMAKE_CURRENT_SOURCE_DIR}/Hello.h")
set(SUBDIRECTORIES "")
SET(RELATIVE_PATH "include/Matrix")


foreach(VAR ${SUBDIRECTORIES})
	add_subdirectory(${VAR})
endforeach()

if(FILES)
	#Add source files to target
	target_sources("${PROJECT_NAME}"  PRIVATE ${FILES})

	#Install our source files
	install(FILES ${FILES} DESTINATION ${RELATIVE_PATH})
endif()