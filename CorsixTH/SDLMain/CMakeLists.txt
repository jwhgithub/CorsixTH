IF(APPLE)
	find_package(SDL2 REQUIRED)

	set(CMAKE_OSX_ARCHITECTURES "x86_64")	
	include_directories(${SDL_INCLUDE_DIR})

	add_library (SDL2main STATIC SDLMain.m)
endif(APPLE)
