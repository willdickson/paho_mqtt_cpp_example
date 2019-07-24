cmake_minimum_required (VERSION 2.6)

project(mqtt_test)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")

set(THREADS_PREFER_PTHREAD_FLAG ON)
find_package(Threads REQUIRED)

add_executable(test main.cpp)

target_link_libraries(test paho-mqttpp3)



