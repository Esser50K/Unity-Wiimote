C# / Unity Wii Remote API
=========================
//Edit Jelle Vermandere 2020

This is an easy to use interface between Unity3D (or C# in general with minimal changes) and a Wii Remote controller.
The library uses a slightly modified version of [Signal11's HIDAPI](https://github.com/signal11/hidapi) to handle
low-level bluetooth communications.  In essence, the API itself is an implementation of the excellent
reverse-engineering effort done at [Wiibrew](http://wiibrew.org/wiki/Wiimote).  Here are some notable features of the
API:

- **Cross Platform**: The API is compatible with Windows (on the Microsoft and BlueSoleil bluetooth stacks), Mac, and
  Linux (only tested on Windows and Mac).
- **Fully Featured**: The API is capable of communicating and interpreting almost all useful data from the Wii Remote,
  including:
    - Basic Button Data (A, B, +, -, 1, 2, D-Pad, Home buttons)
    - 3-Axis Accelerometer reporting
    - IR Camera Data (including pointing position)
    - Extension Controller Support:
        - *Nunchuck*: Joystick data, C and Z buttons, Accelerometer data
        - *Classic Controller*: All Buttons (including analog buttons) and Joysticks
        - *Wii Motion Plus*: Change in Pitch / Yaw / Roll.
        - *Wii U Pro Controller*: All Buttons and Joysticks - The Wii U Pro Controller acts as a Wii Remote with a custom extension controller, so it is compatible with this API.
        - *Guitar Hero Guitar Controller*: All buttons, both strum directions, whammy, slider (touchbar), and analog stick
        - *Wii balance Board*: 4 different pressure values, with calibration mode (currently only relative)
        - *PassthroughMode*: pass through the values of nunchucks and classic controllers while also passing through the motionplus data (tested and works with: "-x0" remotes )
        - More extension controllers coming soon!  Raw data also available for custom extension controllers.
    - Controlling the remote's 4 LEDs
    - Status reporting (battery level, player LED state, etc.)
    - More features coming soon!
- **Fully Documented**: The API comes with an example scene in Unity3D that makes use of all of the API's functions.  The
  API itself is well commented and comes with [Doxygen](http://www.stack.nl/~dimitri/doxygen/) documentation.
- **Open and Growing**: The API is licensed under the generous MIT license (see LICENSE.txt) so you can easily use it
  in your projects.  Source code access lets you debug easier.  Of course, it's also free!

Installation
------------

instal the package from this Repo

