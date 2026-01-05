# trajkit-demo

A small gallery of trajectory and biophysics demo videos and GIFs used in talks, papers, and live walkthroughs, bundled with Sphinx documentation for quick sharing on Read the Docs.

## Quickstart (build docs locally)

```bash
python -m venv .venv
source .venv/bin/activate
pip install -U pip
pip install -r docs/requirements.txt
sphinx-build -b html docs docs/_build/html
```

## Media policy

- Keep each media file under 100 MiB (GitHub rejects larger uploads) and prefer short, looping clips.
- Store assets in `docs/_static/media` using a WebM + MP4 + GIF triad for broad compatibility and previews.
- Use snake_case stems shared across formats (e.g., `example_clip.mp4`, `example_clip.webm`, `example_clip.gif`).

## Demo pages

| Demo | Page | What it shows |
| --- | --- | --- |
| Bacteria 3D Motion | docs/demos/bacteria_3d_motion.rst | 3D trajectories highlighting helical swims and tumbles. |
| Nanorod Membrane Interaction | docs/demos/nanorod_membrane.rst | Anisotropic nanorods bending and adhering to a soft membrane. |
| CDV Correlated Displacement | docs/demos/cdv_correlated_displacement.rst | Correlated displacement vectors for collective dynamics and microrheology discussions. |
