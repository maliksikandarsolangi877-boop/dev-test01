# Plan: Measure It

Object: blue flat square board (size to be measured with ruler)
Reference: expired bank card, flat, same plane (85.6 x 54 mm nominal, measured by me)
Camera: phone, focus/zoom/resolution locked

Order and time budget (8 h):
1. Calibration, 20+ checkerboard images, OpenCV      - 1 h
2. Dataset, 70+ images, CVAT masks, 70/20/10 split    - 2 h
3. Model: Mask R-CNN (torchvision), pretrained backbone, fine-tuned - 2 h (training runs in background)
4. Inference command: undistort, segment, find card, mm output  - 1.5 h
5. Accuracy vs ruler on 10+ instances, raw vs undistorted       - 1 h
6. Docs, README, Loom                                           - 0.5 h

Already decided to skip: items 7 to 10 unless time remains.

Test split: fixed in dataset/splits/test.txt, committed before any code.

Decision record: (written at the end if I reach item 10)