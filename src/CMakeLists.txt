set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -Wno-long-long -pedantic")

# find_package(Boost 1.47 REQUIRED
#   # COMPONENTS ...
#   )
# if(Boost_FOUND)
#   include_directories(${Boost_INCLUDE_DIRS})
add_executable(code                     code.cpp)
# endif()

