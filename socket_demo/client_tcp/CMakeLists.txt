#author   : Liqiang Yang
#e-mail   : tongchi216@163.com
#date     : 2021-1-28
#mender   : 
#e-mail   : 
#date     : 
cmake_minimum_required(VERSION 3.5)

set(sources)
set(includedirs)
set(internal_headers)
set(exported_headers)
set(modulelibs)

add_compile_options(-std=c++11)

list(
    APPEND 
    sources
    ${CMAKE_CURRENT_SOURCE_DIR}/main.cpp
)
link_directories(${LIBRARY_OUTPUT_PATH})

add_executable(client_tcp ${sources})

target_link_libraries(client_tcp)
