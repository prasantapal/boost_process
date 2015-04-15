#!/usr/bin/env bash
project_name=async_io
INCLUDEPATH=/usr/lib/boost
INCLUDEPATHPROCESS=${HOME}/Downloads/process
LIBPATH=/usr/lib/boost/stage/lib
LIBS=-lboost_system 

${project_name}:${project_name}.o
	g++ -o ${project_name} ${project_name}.o -L${LIBPATH} `echo ${LIBS} -lboost_thread`

${project_name}.o:${project_name}.cpp
	g++ -c -I/usr/include/ -I${INCLUDEPATHPROCESS} -I/usr/lib/boost ${project_name}.cpp 
