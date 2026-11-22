# Changes from the original Z-Anatomy template

Base: `Startup.blend` from the Z-Anatomy Blender template (Blender 3.5), processed in Blender 4.5.

## v1.0 (2026-11)

### Removed
Objects identified as coming from non-commercial (NC) sources were deleted:

| Object(s) | Source / licence |
|---|---|
| Cochlea .l/.r, Vestibule .l/.r, Tympanic membrane .l/.r, Cochlear nerve (mesh) | Anatomy of the Inner Ear – University of Dundee – CC BY-NC-SA 4.0 |
| Kidney .l/.r, Renal pelvis .l/.r | Kidney – Lissie Cowley – CC BY-NC 4.0 (removed conservatively) |

Also not exported: text labels, label anchor points (`*.j`), reference lines/planes/movements,
cross-section planes, helper curves (bevel profiles and paths).

Kept (BodyParts3D / Z-Anatomy-made): Malleus, Incus, Stapes, Temporal bone, Auditory tube, the
Z-Anatomy curves `Cochlear nerve.l` and `Vestibulocochlear nerve (VIII)`, ureters, renal vessels,
suprarenal glands.

### Converted and split
- Split into nine files, one per top-level Z-Anatomy collection (body system).
- Curves (vessels, nerves, ureters, etc.) converted to meshes.
- Object rotation/scale baked into vertices (no negative scale); pivots kept at the original object origins.
- Subdivision Surface modifiers **not** applied (base meshes).
- Exported to glTF 2.0 binary (GLB) and FBX, metres, Y-up.
- Materials simplified to base colour only.

### Quest-optimised set only (`*-quest.zip`)
- Curve resolution (`resolution_u` / `bevel_resolution`) reduced before conversion.
- Decimate (collapse) applied to larger objects in the muscular, nervous and cardiovascular files.
- Total ≈ 2.29 M triangles (full set ≈ 9.55 M).

Per-object vertex and triangle counts for both sets are in `manifests/`.
