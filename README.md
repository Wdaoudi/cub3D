# Cub3D

<div align="center">
  <img src="https://img.shields.io/badge/42-Project-blue" alt="42 Project Badge">
  <img src="https://img.shields.io/badge/C-Language-lightgrey" alt="C Language Badge">
  <img src="https://img.shields.io/badge/Raycasting-3D-yellow" alt="Raycasting 3D Badge">
</div>

## 💡 About

Cub3D is a realistic 3D graphical representation of a maze using raycasting principles, inspired by the classic game Wolfenstein 3D. This project renders a dynamic view inside a labyrinth where players must find their way through.

## 🛠️ Usage

### Requirements
* GCC compiler
* Make
* MinilibX library
* X11 include files
* XShm extension

### Instructions

**1. Compiling**
```bash
$ git clone https://github.com/yourusername/cub3D
$ cd cub3D
$ make
```

**2. Running the program**
```bash
$ ./cub3D maps/map.cub
```

## 📋 Features

### Core Features
| Feature | Description |
|---------|-------------|
| Raycasting Engine | 3D visualization using ray-casting technique |
| Textured Walls | Different textures for north, south, east, and west walls |
| Player Movement | Movement using W, A, S, D keys |
| Camera Rotation | Camera rotation using arrow keys or mouse |
| Color Settings | Configurable ceiling and floor colors |
| Map Parsing | Custom .cub map file format parsing |
| Collision Detection | Wall collision handling |

### Bonus Features
* Minimap system for navigation
* Doors that can be opened and closed
* Mouse rotation control
* Collision detection

## ⚙️ Implementation Details

### Architecture
* Map parsing and validation
* Player movement and collision detection
* Raycasting algorithm implementation
* Texture mapping
* Input handling
* Window management

### Technical Choices
* Written in C
* Uses MinilibX for graphical rendering
* Implements efficient raycasting algorithm
* Follows 42 School's Norm

## 🚨 Error Management
* Map validation
* File format checking
* Texture loading verification
* Memory allocation failure handling
* Configuration error detection

## 🗺️ Map Format

The game uses .cub files that define:
* Wall textures (NO, SO, WE, EA)
* Floor and ceiling colors (F, C)
* Map layout using characters:
  * `0` for empty spaces
  * `1` for walls
  * `N`, `S`, `E`, `W` for player starting position and orientation
  * `D` for doors

Example:
```
NO ./textures/north.xpm
SO ./textures/south.xpm
WE ./textures/west.xpm
EA ./textures/east.xpm
F 220,100,0
C 225,30,0

111111111111
100000000001
10000N000001
100000000001
111111111111
```

## 🧪 Controls

* `W`: Move forward
* `S`: Move backward
* `A`: Move left
* `D`: Move right
* `←` `→`: Rotate camera left/right
* `Space`: Interact with doors
* `Enter`: Toggle mouse controls
* `Esc`: Exit game

## 📚 Resources
* [Wolfenstein 3D](http://users.atw.hu/wolf3d/)
* [Raycasting Tutorial](https://lodev.org/cgtutor/raycasting.html)
* [MinilibX Documentation](https://github.com/42Paris/minilibx-linux)

## 🗣️ Contributors

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/Wdaoudi">
        <img src="https://github.com/Wdaoudi.png" width="100px;" alt="wdaoudi-"/>
        <br />
        <sub><b>wdaoudi-</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/luffybzs">
        <img src="https://github.com/luffybzs.png" width="100px;" alt="ayarab"/>
        <br />
        <sub><b>ayarab</b></sub>
      </a>
    </td>
  </tr>
</table>

## 📝 License

This project is [MIT](LICENSE) licensed.
