# Solar System Explorer

An interactive 3D space exploration application built with C++ and OpenGL. Users can pilot a spacecraft through a rendered solar system or switch to an observation mode for a closer view of individual planets.

## Features

- Third-person spacecraft navigation
- Multiple camera and gameplay modes
- Planetary rotation and orbital movement
- Dynamic lighting based on the system’s central light source
- Textured planets, moons, asteroids, and spacecraft models
- Skybox-based space environment
- Imported 3D models using Assimp
- Keyboard and mouse controls

## Gameplay Modes

### Exploration Mode

Exploration Mode allows the user to pilot a spacecraft through the solar system from a third-person camera perspective.

| Input | Action |
|---|---|
| `W` / `S` | Increase or decrease speed |
| `A` / `D` | Turn left or right |
| `Up Arrow` / `Down Arrow` | Pitch the spacecraft |
| `Space` | Brake |
| `Shift` | Accelerate |
| Mouse movement | Steer or adjust the camera |
| `Tab` | Switch to Planetary Observation Mode |

### Planetary Observation Mode

Planetary Observation Mode provides a closer view of a selected celestial body.

| Input | Action |
|---|---|
| Mouse movement | Look around |
| Scroll wheel | Zoom in or out |
| Arrow keys | Move the camera around the target |
| `Tab` | Return to Exploration Mode |

## Technologies

- **C++**
- **OpenGL**
- **GLFW** — window creation and input handling
- **GLEW** — OpenGL extension loading
- **GLM** — graphics mathematics
- **SOIL2** — texture loading
- **Assimp** — 3D model importing
- **Visual Studio**

## Project Structure

```text
solar-system-explorer/
├── src/
│   ├── assets/          # Textures, skybox images, and 3D models
│   ├── camera.cpp       # Camera behavior and movement
│   ├── engine.cpp       # Application and gameplay logic
│   ├── graphics.cpp     # Rendering setup and graphics management
│   ├── mesh.cpp         # Mesh data and rendering
│   ├── object.cpp       # Scene-object behavior
│   ├── shader.cpp       # Shader loading and configuration
│   ├── sphere.cpp       # Planet and sphere geometry
│   ├── window.cpp       # Window and input management
│   └── main.cpp         # Application entry point
├── solar-system-explorer.sln
└── README.md

## Development

This project was developed collaboratively as a two-person computer graphics project. Both team members contributed throughout the design, implementation, debugging, and testing process. Together, we implemented the rendering pipeline, spacecraft navigation, planetary motion, camera systems, lighting, texture mapping, and overall gameplay mechanics.

## Dependencies

- [GLFW](https://www.glfw.org/)
- [GLEW](https://glew.sourceforge.net/)
- [GLM](https://github.com/g-truc/glm)
- [SOIL2](https://github.com/SpartanJ/SOIL2)
- [Assimp](https://assimp.org/)

## Future Improvements

- Add cross-platform build support
- Improve spacecraft controls and camera transitions
- Add a planet-selection interface
- Improve physical scaling and orbital behavior
- Add automated build validation