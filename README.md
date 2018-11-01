# Particle Life

A game of life using particles, instead of cells.

A JavaScript conversion, based on [Particle-Life](https://github.com/HackerPoet/Particle-Life) by [HackerPoet](https://github.com/HackerPoet).

[See it in the browser][demo]

## Todo

- [ ] Optimize rendering
    - Perhaps switch from `canvas-sketch` to a more stable and performant library (or home-grown)
- [ ] Further optimize the algorithm.
    - Use fixed-size data structures instead of arrays?
    - Allocate as much during initialization, before rendering.
    - Measure and optimize `Universe.step()` function.
    - Measure random-js and prob.js performance to ensure it is not a huge bottleneck.

## Known Bugs

- Rendering performance is currently pretty poor (18-20 fps).
- There's no keymapping for zooming / reset, yet.

## Probable bugs

- With current seed, particles will create huge lumps. This may or may not be intended. Look into attraction algorithm and/or the randomness behind it.

## Ideas

- [ ] Port the C++ code to WASM using Emscripten.

[demo]: https://whatever.io