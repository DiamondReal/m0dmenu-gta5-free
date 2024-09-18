# caustics-display

A simple C++ program used to verify the caustics pattern produced by the output of [Kassubeck et al.'s implementation](https://github.com/CompN3rd/ShapeFromCaustics/tree/main/schwartzburg_2014) of Schwartzburg at al.'s [High-contrast computational caustic design](https://dl.acm.org/doi/10.1145/2601097.2601200).

## Dependencies

Make sure to include these when building the program.
- [SDL 2](https://www.libsdl.org/)
- [Eigen](https://eigen.tuxfamily.org/)

## How to use

1. First build the caustics display executable.
2. Run Kassubeck at al.'s implementation to obtain an .obj file for your target image. The target image must be 256x256 pixels.
3. Place the .obj file in the same directory as the built executable.
4. Open the command line in the same directory, and run:
`causticsdisplay.exe [filename].obj [receiver_plane]`
<br>The first argument is the .obj file, and the second argument is the distance to the receiver plane when generating the .obj file.
5. If successful, the display window will open and the caustics pattern will be shown.
<br>The window can be resized to make the pattern more clear.
<br>Pressing the W and S keys will increase or decrease the receiver plane distance, respectively, in order to fine-tune the spacing.
<br>Pressing Q will display the current distance.

## Screenshots