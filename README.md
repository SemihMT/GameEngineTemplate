# Game Engine Template
This repository is one I created to decrease the amount of boilerplate necessary to start a game/engine project. 

The built application consists of a static library that includes SDL2 and an executable that starts a window.

## Requirements
This project depends on SDL2 being discoverable by CMake. I've used the `find_package` command to link SDL2 to the engine. So make sure there is a local copy of SDL2 in your `CMAKE_PREFIX_PATH` environment variable.

## Building the project
Following the usual CMake build steps should suffice.

### Clone the repo
```bash
git clone https://github.com/SemihMT/GameEngineTemplate.git
```
### Create a build directory
It's a good practice to create a separate build directory to keep the source files clean:
```bash
mkdir build 
cd build
```
### Configure the project
```bash
cmake ..
```
### Build the project
```bash
cmake --build .
```