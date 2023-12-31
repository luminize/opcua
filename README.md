# opcua
OPC UA module for the Godot game engine

installation of 3rd party OPC-UA library

cd open62541
git submodule update --init --recursive

thus pulls and updated the submodule

mkdir build

cmake-gui

set correct source code directory and build directory
build_shared_libs
ua_enable_amalgamation
configure for your latest MS Visual Studio release and generate

cd build

RMC the open62541.sln file, make sure it is with the MS Visual Studio version you configured for in the cmake step

RMC on "ALL_BUILD" and build.

this should now have made all the files you need in the open62541 submodule

copy from the directory open62541/open62541.h/.c to a new directory shared_62541
copy contents open62541/build/bin/Debug that got generated to the directory shared_62541