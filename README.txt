FOUR-WAY TRAFFIC SIGNAL SIMULATOR

PROJECT OVERVIEW This project is a 2D Four-Way Traffic Signal Simulator
developed in C using OpenGL, FreeGLUT and GLU. It displays a four-way
road junction, traffic signals, moving vehicles and a control panel for
changing signal states.

TECHNOLOGIES USED - C programming language - OpenGL (legacy
fixed-function pipeline / immediate-mode rendering) - FreeGLUT (window
creation and input handling) - GLU (2D orthographic projection)

MAIN FEATURES - Four-way road junction - Four directional traffic
signals - Manual signal control using on-screen buttons - Random vehicle
generation - Vehicle movement based on signal state - Vehicle spacing to
reduce overlapping - Live vehicle count and passed-vehicle statistics -
Pause, resume, reset and speed controls

CONTROLS - Spacebar: Pause or resume - R: Reset the simulation - + or =:
Increase vehicle speed - - or _: Decrease vehicle speed - Up Arrow:
Increase vehicle speed - Down Arrow: Decrease vehicle speed - Left mouse
click: Select a Red, Yellow or Green signal button - Esc: Exit the
application

REQUIREMENTS - Windows - GCC compiler from MSYS2 UCRT64 - FreeGLUT
development package - OpenGL and GLU libraries

INSTALL FREEGLUT Open the MSYS2 UCRT64 terminal and run:

pacman -S mingw-w64-ucrt-x86_64-freeglut

BUILD THE PROGRAM Open the VS Code terminal in the folder containing
traffic_simulator_opengl.c and run:

gcc traffic_simulator_opengl.c -o traffic.exe -lfreeglut -lopengl32
-lglu32 -lm

RUN THE PROGRAM In PowerShell, run:

..exe

OPENGL CONCEPTS DEMONSTRATED - 2D coordinate system using gluOrtho2D() -
Primitive drawing using GL_QUADS, GL_LINES, GL_LINE_LOOP and
GL_TRIANGLE_FAN - Colour selection using glColor3f() - Vertex
specification using glVertex2f() - Double buffering using
glutSwapBuffers() - Display, reshape, mouse, keyboard and timer
callbacks

PROJECT NOTES This project uses legacy immediate-mode OpenGL with the
fixed-function pipeline. FreeGLUT manages the application window and
input callbacks. GLU provides the 2D orthographic projection.

This simulator is a visual demonstration and is not a real-world traffic
control system.
