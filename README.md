# SwlFT-YOLO

## Contents

- `SWlFT-YOLO.yaml`: model configuration (Ultralytics 8.3.68)
- `module/`: DownWT, C2f_ScConv and BiFPN implementations
- `Module Example/weights/`: trained weights (`best.pt`, `last.pt`)
- `Module Example/`: training curves and validation previews;

Note: `best.pt` was trained with a single class. Parameter and FLOP counts in the paper followed the official Ultralytics model cards. Running `best.pt` requires the SwlFT module, which will be released after acceptance.


## Coming after acceptance

- SwlFT source code
- Training, evaluation and inference scripts
- TensorRT FP16 export and Jetson deployment scripts
