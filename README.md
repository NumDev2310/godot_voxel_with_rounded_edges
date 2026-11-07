# GodotVoxel with Rounded Edges

This fork of [Zylann's Voxel Tools for Godot](https://github.com/Zylann/godot_voxel) adds optional rounded edges and corners to blocky terrain, including the underside.
Rounding is off by default: enable `rounding_enabled` on selected cube models in the existing `VoxelBlockyLibrary` or `VoxelBlockyTypeLibrary` arrays.

Shared library controls set the bevel amount, transition length, and linear or nonlinear taper profile. Rounded corner caps blend into connected edges, while blocked contacts taper back to square edges.

Use `rounding_affects_neighbors` to let decorations or water count as air for neighboring bevels while keeping those models unrounded. The feature supports full unit cubes and compatible imported cube meshes; other shapes retain their original geometry.

| Rounded edges | Original edges |
|:---:|:---:|
| <img src="https://github.com/user-attachments/assets/1c639c15-1341-4f11-9750-fc086a8d0268" alt="Rounded terrain" width="600"> | <img src="https://github.com/user-attachments/assets/f2ef664e-51d9-42d5-9aa9-dcd46bbd814e" alt="Original terrain" width="600"> |
| <img src="https://github.com/user-attachments/assets/ceedc5dc-ec98-45ee-8c97-e0d78326742c" alt="Rounded terrain, second view" width="600"> | <img src="https://github.com/user-attachments/assets/062c8c4a-034b-442a-a6a4-464a3d48b0b2" alt="Original terrain, second view" width="600"> |


See the [rounding guide](doc/source/blocky_rounding.md) for setup and limitations.
Upstream documentation, credits, and supporter acknowledgments in [README.upstream.md](README.upstream.md), and the original [MIT license](LICENSE.md) remains unchanged.
