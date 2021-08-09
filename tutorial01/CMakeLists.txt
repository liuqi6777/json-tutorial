cmake_minimum_required (VERSION 3.0.0)
project (leptjson_test C)

set(CMAKE_CXX_FLAGS ${CMAKE_CXX_FLAGS} -g)
set(LIB_SRC leptjson.c)
set(APP_SRC test.c)

add_library(leptjson ${LIB_SRC})
add_executable(${PROJECT_NAME} ${APP_SRC})
target_link_libraries(leptjson_test leptjson)
