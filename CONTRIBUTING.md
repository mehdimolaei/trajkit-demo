# Contributing

Thanks for helping expand the demo gallery. This repository is focused on media and documentation, not a full Python package.

## Add a new demo
1. Place `*.gif`, `*.mp4`, and `*.webm` files in `docs/_static/media` using the same stem and snake_case naming.
2. Create a new `docs/demos/<name>.rst` page with a short description, preview GIF, and embedded video block.
3. Add the page to `docs/demos/index.rst` so it appears in the gallery and build output.

## Naming and size rules
- Use snake_case stems shared across all three formats (e.g., `sample_demo.mp4`, `sample_demo.webm`, `sample_demo.gif`).
- Keep individual files under 100 MiB to stay within GitHub limits.
