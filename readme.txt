Assignment 3 – Image Stitching & Feature Matching
Computer Vision • Spring 2024 – Vijay Hooda (2021365)

├─ Assignment_3_VH_2021365.pdf          – detailed report, experiments, and panoramas
├─ 2.py                                 – end-to-end panorama pipeline (feature match → RANSAC homography → multi-band blend)
├─ 2.ipynb                              – notebook walkthrough of 2.py with visuals
├─ brute_feature_matching/              – key-point matches using BF-SIFT (PNG/JPG outputs)
├─ flann_feature_matching/              – key-point matches using FLANN-SIFT
├─ blended_img/                         – final panoramas produced by multi-band blending
├─ images/                              – input image sequence (frame_*.jpg)
└─ utils.py                             – helper functions (image I/O, blending, visualization)

Quick Run
---------
python 2.py --img_glob "images/frame_*.jpg" --output panorama.jpg --blend multi
