# Project definition — Harvest December: Reharvested! Portable

## Product and boundary
A collaborative portable Ren'Py port snapshot for **Harvest December: Reharvested!**, with a Vita package tree under `PSVITA Port/`. This repository is related to the upstream portable project and must not be treated as the authoritative source for the original game.

## Upstream and provenance
- Project/upstream collaboration: [takoyaki99/Harvest-December-Reharvested-Portable](https://github.com/takoyaki99/Harvest-December-Reharvested-Portable).
- The README credits Autumn Rivers' PC rework as the basis for the port.
- Original game assets and third-party runtime components require their own licensing/provenance checks before redistribution.

## Users and target
PS Vita first; the README mentions Nintendo Switch as a possible parallel target, but this repository's current tracked package path is the Vita tree. Do not infer Switch release readiness from Vita metadata.

## Architecture and dependencies
The tree contains a nested `PSVITA Port/` package with `eboot.bin`, `renpy.py` and `sce_sys/`, plus a root-level `renpy.py`. The relationship between root and nested runtime copies must be clarified before packaging. The original game data and upstream port sources remain dependencies.

## Security and quality
Validate the nested Vita SFO/LiveArea package. Track source attribution and license notices for runtime and assets. Avoid overwriting upstream work or claiming that the root and nested runtime copies are interchangeable.

## Verified baseline
The Git tree contains a Vita package subtree and project/wiki documentation. This inventory does not prove a current Vita boot, a Switch build, or the provenance of every bundled binary.

## Release acceptance
Document the authoritative runtime tree, pass package integrity checks, verify licenses and upstream revisions, then test installation, boot, gameplay, save/load and suspend/resume on real Vita hardware. Any Switch target requires its own separate build and hardware evidence.