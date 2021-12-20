set(SOURCES
	main.cpp
)

find_package(SFML 2.5 COMPONENTS graphics window system network audio REQUIRED)

add_executable(${CMAKE_PROJECT_NAME} ${SOURCES})

target_link_libraries(${CMAKE_PROJECT_NAME} 
  sfml-graphics
  sfml-window 
  sfml-system 
  sfml-network 
  sfml-audio
)