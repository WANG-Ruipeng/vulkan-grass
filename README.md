Vulkan Grass Rendering
==================================

**University of Pennsylvania, CIS 565: GPU Programming and Architecture, Project 5**

**Demo**:



https://github.com/WANG-Ruipeng/vulkan-grass/assets/98011585/073ff7da-813b-45c1-991e-1897d8ea6a51

#### How to build on Windows

1. In Git Bash, navigate to your cloned project directory.
2. Create a `build` directory: `mkdir build`
   * (This "out-of-source" build makes it easy to delete the `build` directory and try again if something goes wrong with the configuration.)
3. Navigate into that directory: `cd build`
4. Open the CMake GUI to configure the project:
   * `cmake-gui ..` or `"C:\Program Files (x86)\cmake\bin\cmake-gui.exe" ..`
     * Don't forget the `..` part! This tells CMake that the `CMakeLists.txt` file is in the parent directory of `build`.
   * Make sure that the "Source" directory points to the directory `cuda-getting-started`.
   * Click *Configure*.
      * Select your Visual Studio version (2019 or 2017), and `x64` for your platform. (**NOTE:** you must use x64, as we don't provide libraries for Win32.)
   * Click *Generate*.
5. If generation was successful, there should now be a Visual Studio solution (`.sln`) file in the `build` directory that you just created. Open this with Visual Studio.
6. Build. (Note that there are Debug and Release configuration options.)
7. Run. Make sure you run the `cis565_` target (not `ALL_BUILD`) by right-clicking it and selecting "Set as StartUp Project".
   * If you have switchable graphics (NVIDIA Optimus), you may need to force your program to run with only the NVIDIA card. In NVIDIA Control Panel, under "Manage 3D Settings," set "Multi-display/Mixed GPU acceleration" to "Single display performance mode".

#### Interaction
Left click and move around to move the camera.  
Right click and move around to move the collision object.  
Scroll up and down to move closer or further.  
Click and scroll the mouse wheel to change the size of the collision object.
