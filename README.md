# GodotVoxel with Rounded Edges

This fork of [Zylann's Voxel Tools for Godot](https://github.com/Zylann/godot_voxel) adds optional rounded edges and corners to blocky terrain, including the underside.
Rounding is off by default: enable `rounding_enabled` on selected cube models in the existing `VoxelBlockyLibrary` or `VoxelBlockyTypeLibrary` arrays.
Shared library controls set the bevel amount, transition length, and linear or nonlinear taper profile.
Rounded corner caps blend into connected edges, while blocked contacts taper back to square edges.
Use `rounding_affects_neighbors` to let decorations or water count as air for neighboring bevels while keeping those models unrounded.
The feature supports full unit cubes and compatible imported cube meshes; other shapes retain their original geometry.
See the [rounding guide](doc/source/blocky_rounding.md) for setup and limitations.
Upstream documentation, credits, and supporter acknowledgments are preserved in [README.upstream.md](README.upstream.md), and the original [MIT license](LICENSE.md) remains unchanged.
