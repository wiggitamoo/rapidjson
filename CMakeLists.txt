cmake_minimum_required(VERSION 3.14)

include("cmake/HunterGate.cmake")
HunterGate(
		URL "https://github.com/ruslo/hunter/archive/v0.16.15.tar.gz"
		SHA1 "6974c2150fc0d3b09de3ad1efcbf15d360647ffa"
)

project(rapidjson)

set(CMAKE_CXX_STANDARD 17)

add_executable(rapidjson main.cpp)

#hunter_add_package(RapidJSON)
#find_package(RapidJSON CONFIG REQUIRED)
#target_link_libraries(rapidjson RapidJSON::rapidjson)
