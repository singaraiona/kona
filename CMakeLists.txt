cmake_minimum_required(VERSION 2.8)
project(kona)
include_directories("src/")
set(SOURCES test.cpp lib1.cpp lib2.cpp)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 -Wall -lm -ldl")
set(SOURCES src/0.c src/d.c src/kapi.c src/k.c src/kg.c src/kn.c src/ks.c src/main.c src/p.c src/v.c src/vd.c src/vg.c src/c.c
 src/getline.c src/kc.c src/km.c src/ko.c src/kx.c src/mt.c src/r.c src/va.c src/vc.c src/vf.c src/vq.c)
add_executable(k ${SOURCES})
target_link_libraries(k "-lm -ldl")