# Anatomy Digital — 3D anatomy models (CC BY-SA 4.0)

These are the 3D human anatomy models used in **Anatomy Digital**, a VR/MR anatomy app for Meta Quest
by Arjun Technology (https://anatomy.arjuntech.id).

They are an **adapted version** of the Blender template of **Z-Anatomy – The libre 3D atlas of anatomy**
(https://github.com/Z-Anatomy/Models-of-human-anatomy), which itself is largely derived from
**BodyParts3D** (The Database Center for Life Science). They are published here, free and without DRM,
under the same licence as the original: **Creative Commons Attribution-ShareAlike 4.0 International
(CC BY-SA 4.0)** — see [`LICENSE`](LICENSE).

> This is not an official Z-Anatomy or BodyParts3D release, and neither project endorses
> Anatomy Digital or Arjun Technology.

## Downloads

The model files are attached to each **GitHub Release** (not stored in the repository itself):

| File | Contents |
|---|---|
| `anatomy-digital-models-v1.0-quest.zip` | **Exactly the meshes shipped in the app** (Quest-optimised): GLB + FBX per body system, ≈2.29 M triangles in total |
| `anatomy-digital-models-v1.0-full-glb.zip` | Full-resolution base meshes, GLB per body system, ≈9.55 M triangles in total |

Each release version matches the app version that uses those models.

## Files per release

Nine files, one per body system (same split as in the app):

| File | System | Objects |
|---|---|---:|
| `01_skeletal` | Skeletal system | 278 |
| `02_muscle_insertions` | Muscular insertions | 705 |
| `03_joints` | Joints & ligaments | 414 |
| `04_muscles` | Muscular system | 684 |
| `05_cardiovascular` | Cardiovascular system | 676 |
| `06_lymphoid` | Lymphoid organs | 164 |
| `07_nervous_sense` | Nervous system & sense organs | 576 |
| `08_visceral` | Visceral systems | 117 |
| `09_regions` | Regions of the human body | 257 |

- Units: metres, Y-up. GLB is glTF 2.0 binary; FBX uses -Z forward / Y up.
- One node = one anatomical structure, named with the original (Terminologia Anatomica-style) English
  name from Z-Anatomy, with `.l` / `.r` suffixes for left / right.
- `manifests/` lists every object per file: source type (mesh or curve), collection path, vertices, triangles.
- Only base colours are included; the original Z-Anatomy shaders are not.

## Attribution

When you reuse these models, please credit (see [`ATTRIBUTION.md`](ATTRIBUTION.md) for details):

> Z-Anatomy – The libre 3D atlas of anatomy – CC BY-SA 4.0
> BodyParts3D – The Database Center for Life Science – CC BY-SA 2.1 Japan
> Adapted by Arjun Technology for Anatomy Digital – CC BY-SA 4.0

Any adaptation you distribute must also be licensed under CC BY-SA 4.0 (or a compatible licence).

## What we changed

See [`CHANGES.md`](CHANGES.md).

## Not included

- The Anatomy Digital app, its source code, and its other content (text, audio, UI) — these are not
  part of this release and are not covered by this licence, except where stated in the app's credits.
- Models licensed for **non-commercial use only** in the Z-Anatomy template (inner ear and kidney models) — removed.
- Text labels, label anchors, Wikipedia definitions and Blender scripts from the Z-Anatomy template.

## Medical disclaimer

These models are for education only. They are simplified and may contain inaccuracies; they are not
intended for diagnosis, treatment or surgical planning.

## Contact

admin@arjuntech.id · https://anatomy.arjuntech.id/support.html
