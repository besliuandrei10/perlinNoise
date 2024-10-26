# Introduction #
Perlin noise is a type of gradient noise used in computer graphics to create natural-looking textures and patterns, such as clouds, landscapes, and fire. Developed by Ken Perlin in 1983, it produces a smooth, continuous noise pattern that avoids the harsh randomness of traditional white noise by blending gradients between nearby points. This results in a more organic, cohesive look, which is especially valuable in procedural generation for visual effects and 3D rendering. Perlin noise is computationally efficient and can be layered at different scales to create complex, multi-textured surfaces that enhance realism in digital art and simulations.

# Description #

Perlin noise is calculated by generating a pseudo-random, smooth gradient field across a grid and interpolating between these gradients to create smooth transitions. Here is a breakdown of the process:

- **Grid Definition**:
    A fixed size grid is defined where each intersection has a randomly selected unit-length vector.
    ![alt text](img/PerlinNoiseGradientGrid.svg)
- **Dot Product**: Each output cell has it's value computed using the associated unit-length vectors found in the previously defined grid.
    ![alt text](img/PerlinNoiseDotProducts.svg)
- **Interpolation**: The result is then interpolated in order to smooth out transitions and provide a cleaner, more natural output.
    ![alt text](img/PerlinNoiseInterpolated.svg)

By repeating this process at multiple points and combining these layers at different frequencies and amplitudes (octaves), Perlin noise can be scaled to produce various textures from soft, low-frequency patterns to complex, high-frequency details.

# Objective #

Our objective is to take an already existing perlin noise implementation and paralelize it using different means in order to improve performance and compare the efficiency of our different solutions. Namely we will use _Intel's Threading Building Blocks (TBB)_, ***TBD*** and ***TDB***

#  #

# Resources #
- Perlin noise implementation:
https://github.com/Maharshi-Pandya/Perlin-Noise-Implementation
- Perlin Noise Wikipedia article:
https://en.wikipedia.org/wiki/Perlin_noise