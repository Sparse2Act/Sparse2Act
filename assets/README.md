# Sparse2Act Website Assets

Published website assets use the following structure:

```text
assets/images/teaser-masked-tokenization.png

assets/pointclouds/{task}/sim.ply
assets/pointclouds/{task}/real.ply

assets/videos/{task}/trial-01.mp4
assets/videos/{task}/trial-02.mp4
assets/videos/{task}/trial-03.mp4
assets/videos/{task}/trial-04.mp4

assets/videos/opening/frame-01.mp4
assets/videos/opening/frame-02.mp4
assets/videos/opening/frame-03.mp4
assets/videos/opening/frame-04.mp4

assets/videos/project-overview.mp4
assets/videos/sim-to-real-comparison.mp4
```

Published videos are H.264 MP4 files with web-optimized metadata and fast-start
layout. Trial and opening videos are silent.

An optional `.jpg` poster can accompany every MP4 using the same basename, for
example `trial-01.jpg`.

Task directory names:

```text
bin-picking
cube-stacking
mug-plate
mug-toy
```

Use H.264 MP4 videos and PLY point clouds containing XYZ coordinates with
optional RGB vertex colors. The simulation result charts are inline SVG elements
in `index.html` and do not require image assets.

Original exports, archives, and raw intermediate files are stored locally under
`.source-assets/`, which is intentionally excluded from Git.
