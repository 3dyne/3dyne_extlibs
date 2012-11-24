

include_directories( include )

FILE(GLOB SRC 
	src/*.c
	src/audio/*.c
	src/cdrom/*.c
	src/cpuinfo/*.c
	src/events/*.c
	src/file/*.c 
	src/joystick/*.c
	src/stdlib/*.c 
	src/thread/*.c 
	src/timer/*.c 
	src/video/*.c 
	src/audio/windib/*.c
	src/video/windib/*.c 
	src/video/wincommon/*.c 
	src/joystick/win32/*.c
	src/cdrom/win32/*.c
	src/thread/win32/*.c
	src/timer/win32/*.c 
	src/loadso/win32/*.c )


add_library( SDL ${SRC} )