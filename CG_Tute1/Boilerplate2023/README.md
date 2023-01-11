# OpenGL boilerplate

## Contents
- glfw, glad and glm built from source in `libraries`

- Standard shader class from learnopengl.com and stb_image.h in `include`

- CMake file to compile project (includes glfw, glad, glm and freetype)


## Instructions to build

1. <b>INITAL SETUP</b> (do this once)

    - Setup FreeType to render text 
        - Linux/macOS (recommended OSes)
            - Download the latest stable release(2.10.1) from [the official website](https://freetype.org/download.html)
            - Run the following
                1.  `tar -xvf freetype-2.10.1.tar.gz`
                2.  `cd freetype-2.10.1`
                3.  `./configure --prefix=/usr/local/freetype/2_10_1 --enable-freetype-config` : Prefix defines where freetype is installed
                4.  `make; make install`
        - Windows
            - Use [this video](https://www.youtube.com/watch?v=qW_8Dyq2asc) if using VSCode (I hope you aren't)

2. `mkdir build; cd build`
3. `cmake ..; make`
