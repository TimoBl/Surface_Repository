# Surface Repository

author: Timo Blattner\
date: 26.02.2025\

This repository contains the tracings, surface reconstructions and results for our brain collection. The metadata include an overview of the species, sequences and tracings


## Tracings

Here are all the manual tracings done with Osirix which we relied on for the project. Each scans has tracings of one hemisphere for the pial surface (GM), white matter surface (WM), cerebellum (CEREBELLUM). We also have a broad reconstruction of the hull (OUTER), and the tracings might include other tracings with are not relevant

## Surface Results

These surfaces were generate using a [https://github.com/TimoBl/Few-Shot-Cortex](few-shot-reconstruction-method). Here we have the results for each hemisphere as a surface file.
* .pial : pial surface
* .white : white matter surface
* .exp : exposed surface using a rolling ball method
* .convex : convex full of the pial surface

We also have point wise thickness measurement using DiReCT's integration (thickness_direct) and FreeSurfer thickness (thickness_fs), which can be overlayed to the surface. Surface can be viewed with Freeview as followed

```
freeview -f *.white rh.pial:overlay=rh_thickness_direct lh.pial:overlay=lh_thickness_direct 
```

We also have the results which were extracted directly from the surface (results_surf.csv), and the ones from the segmentation and direct (results_direct.csv)
