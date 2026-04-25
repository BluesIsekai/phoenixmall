# Phoenix
Phoenix is an open-source 3D simulation project. Built with modern OpenGL (core profile), the project is designed for immersive graphics programming and rendering.

## Features
- Custom shader pipeline for advanced rendering.
- Input handling with frame-independent processing.
- Extensible architecture for adding new features and components.
- Phong Lighting is used for lighting the scene.
- Reflections are used in the storefronts and the outside world like cars, ground, etc...
- Blending is used for drawing transparent objects.
- Instancing is used for increasing performance.
- MSAA (Multisample Anti-Aliasing) is used for a better 3D graphics experience.
- Cubemaps used for skybox and reflections.
- Depth testing to prevent objects from rendering in the front while they're supposed to be behind other objects.
- 3D audio using the irrKlang library for a better 3D experience.
- transformations for objects like an elevator, escalators, cars, etc...
- Day/night mode.
- A camera with two modes: Free Camera (First-Person View) and fly mode.
- And more...

## Prerequisites
Before building Phoenix, ensure you have the following installed on your system:

- A C++17-compatible compiler
- CMake (minimum version 3.16)
- git

Platform notes:
- Linux: install OpenGL, X11, GLFW3, ASSIMP development packages if they are not already available.
- Windows: use Visual Studio 2022 or MinGW-w64, and ensure GLFW3/ASSIMP are discoverable.
- macOS: build is supported, audio is disabled by default in CMake.

## Building the Project

### Windows
1. Clone the repository:
   ```sh
   git clone https://github.com/BluesIsekai/phoenixmall.git
   cd phoenixmall 
   ```
2. Configure and build:
   ```sh
   mkdir build
   cd build
   cmake ..
   cmake --build . --config Release
   ```
3. The executable is generated in `bin` as `Phoenix.exe`.

### Linux
1. Clone the repository:
   ```sh
   git clone https://github.com/BluesIsekai/phoenixmall.git
   cd phoenixmall
   ```
2. Configure and build:
   ```sh
   mkdir build
   cd build
   cmake ..
   cmake --build . -j
   ```
3. The executable is generated in `bin` as `Phoenix`.

### MacOS
1. Follow the Linux instructions.
2. Audio is optional and disabled by default on macOS in the current CMake configuration.

## Usage
1. Run the generated executable from the `bin` directory:
   ```sh
   ./Phoenix
   ```
2. Use the following controls to interact with the application:
   - **W/A/S/D**: Move the camera
   - **Mouse**: Look around
   - **LEFT_MOUSE_BOTTUN**: toggle light mode.
   - **RIGHT_MOUSE_BOTTUN**: toggle camera mode.
   - **KEY_0 & KEY_1 & KEY_2**: to use elevator between the ground, first and second floor. 
   - **ENTER**: to enter or get out of the Lamborghini.
   - **SHIFT**: to run.

## Project Structure
- **src/**: Contains the source code for the application
- **includes/**: Header files and third-party libraries
- **resources/**: Models, textures, and shaders used in the simulation
- **cmake/**: CMake modules for finding dependencies
- **bin/**: Compiled executables and resources

---

Enjoy exploring Phoenix Mall in 3D!

