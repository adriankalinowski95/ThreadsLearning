cmake_minimum_required(VERSION 3.28)

project(threads_learning)

set (CXX_FLAGS "-Wall")
set (CMAKE_CXX_FLAGS, "${CXX_FLAGS}")
set (CMAKE_BUILD_TYPE Debug)

set (THREADS_LEARNING_TARGET "threads_learning")

set (SOURCE_FILES 
    main.cpp
)

add_executable(${THREADS_LEARNING_TARGET} ${SOURCE_FILES})

set(CMAKE_CXX_STANDARD 20)

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET ${THREADS_LEARNING_TARGET} PROPERTY CXX_STANDARD 20)
endif()

#target_link_libraries(${THREAD_LEARNING_TARGET} PRIVATE )

