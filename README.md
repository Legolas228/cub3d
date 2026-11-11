# cub3D

A small 3D raycasting project written in C as part of the 42 curriculum. It renders a 3D-style view of a maze using a 2D map, textured walls and the miniLibX graphics library. The project is inspired by the early first-person games such as Wolfenstein 3D.

## My contribution

This was a collaborative project. I was primarily responsible for the parsing part, handling the configuration file and map data before they were used by the game.

This included interpreting texture paths and floor/ceiling colours, processing the map layout and checking that the map data followed the expected format.

## Features

- 3D rendering based on a 2D map
- DDA raycasting
- Textured walls with separate textures for each direction
- Configurable floor and ceiling colours
- Player movement and camera rotation
- Map and configuration loading from `.cub` files
- Map validation

## Technologies

- C
- miniLibX
- DDA raycasting
- 2D map parsing and validation
- Make

## Installation and usage

Compile the project:

```bash
make
```

Run the program with a map file:

```bash
./cub3D maps/map.cub
```

## Controls

- `W`, `A`, `S`, `D`: Move
- Arrow keys: Rotate the camera
- `ESC`: Exit

## Map configuration

The `.cub` file contains the texture paths, floor and ceiling colours, and the map layout.

Example:

```text
NO ./path_to_north_texture.xpm
SO ./path_to_south_texture.xpm
WE ./path_to_west_texture.xpm
EA ./path_to_east_texture.xpm
F 220,100,0
C 225,30,0

111111
100001
101101
1N0111
111111
```

## Context

cub3D was developed as a team project at 42. Its main goal was to explore basic graphics programming, raycasting and the processing of structured map data in C.
