cmake_minimum_required (VERSION 3.8.2)

project (CppProjectTemplate)

if(${CMAKE_CXX_COMPILER_ID} STREQUAL MSVC)
	set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} /W4 /std:c++17")
elseif( ${CMAKE_CXX_COMPILER_ID} STREQUAL "GNU"  )
	set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wextra -std:c++17")
endif()

add_subdirectory (SampleProject)