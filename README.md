GDNative C++ Example
====================

This repository contains the example GDNative C++ library in support of this tutorial:
http://docs.godotengine.org/en/latest/tutorials/plugins/gdnative/gdnative-cpp-example.html


# USAGE

## Requeriments

Depending on your OS there will be different ways of installing this tools

    * git (https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
    * scons (https://scons.org/)
    * a C++ compiler 

## TL;TR Linux example

    git clone https://github.com/jmrepetti/gdnative_cpp_example.git
    cd gdnative_cpp_example 
    git clone --recursive -b 3.3 https://github.com/godotengine/godot-cpp
    cd godot-cpp
    scons platform=linux generate_bindings=yes -j4
    cd ..    
    scons platform=linux

Import the project under 'demo' folder with Godot Editor and Run.


## Clone this repository

    git clone https://github.com/jmrepetti/gdnative_cpp_example.git

## Build C++ bindings

https://docs.godotengine.org/en/stable/tutorials/plugins/gdnative/gdnative-cpp-example.html#building-the-c-bindings

    cd gdnative_cpp_example 
    git clone --recursive -b 3.3 https://github.com/godotengine/godot-cpp

If you have your own custom build Godot, you may need to regenerate API metadata (follow the tutotial link above)

Build the bindings for your platform (replacing \<platform\> with **windows**, **linux** or **osx** depending on your OS):

    cd godot-cpp
    scons platform=<platform> generate_bindings=yes -j4
    cd ..

You may need to add bits=64 to the command on Windows or Linux.

## Creating a simple plugin

https://docs.godotengine.org/en/stable/tutorials/plugins/gdnative/gdnative-cpp-example.html#creating-a-simple-plugin


## Compiling the plugin 

https://docs.godotengine.org/en/stable/tutorials/plugins/gdnative/gdnative-cpp-example.html#compiling-the-plugin

You'll probably need to run this step every time you update your c++ code.

    scons platform=<platform>

Here, we've compiled both godot-cpp and our gdexample library as debug builds. For optimized builds, you should compile them using the target=release switch.

## Using the GDNative module

https://docs.godotengine.org/en/stable/tutorials/plugins/gdnative/gdnative-cpp-example.html#using-the-gdnative-module

## Open the project with Godot

Open Godot editor and import the project under *demo* folder
