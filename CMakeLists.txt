include_directories(${CMAKE_CURRENT_SOURCE_DIR}/include)
file(GLOB_RECURSE WIN_PTHREAD_SOURCE "${CMAKE_CURRENT_SOURCE_DIR}/*.c")
file(GLOB_RECURSE WIN_PTHREAD_HEADER "${CMAKE_CURRENT_SOURCE_DIR}/*.h")
add_library(winpthreads STATIC ${WIN_PTHREAD_SOURCE} ${WIN_PTHREAD_HEADER})

add_definitions(-D_DEBUG)
add_definitions(-D_CONSOLE)
add_definitions(-D_MBCS)
