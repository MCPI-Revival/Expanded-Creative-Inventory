# MCPI-Better-Creative-Inventory
This is a mod for [MCPI-Reborn](https://gitea.thebrokenrail.com/TheBrokenRail/minecraft-pi-reborn) that expands the "Expand Creative Inventory" mod even more, so that you have access to all items in the game.

## Using
To use this mod you will need to download the shared library and place it in the mods folder of minecraft: pi edition, to do this download libbci.so and run 
```bash
wget https://github.com/MCPI-Revival/Expanded-Creative-Inventory/raw/main/libbci.so -o /opt/minecraft-pi-reborn-client/mods/libbci.so 
``` 
Then all you need to do is run minecraft: pi edition with the "Expand Creative Inventory" feature activated. If you are using a launcher such as gMCPIl or jMCPIL, you'll want to enable it in the "Features" tab and launch with "Custom Profile" for the profile selection.

## Compiling
To compile your own version of it you will need the libreborn folder and the creative.cpp file, then once you finish editing creative.cpp, you run:
```bash
arm-linux-gnueabihf-g++ -shared -o libbci.so creative.cpp -DREBORN_HAS_COMPILED_CODE
``` 
This will compile a version of libbci.so with your changes.
