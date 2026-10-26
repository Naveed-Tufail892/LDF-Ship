LDF-Ship
LDF-Ship is a lightweight RT-DETRv4-based detector for ship detection in optical and SAR imagery. It combines a compact two-scale feature hierarchy with LDEM, LWFM, NWD–Shape localization, and IoU-gated Dense-Positive supervision.
Datasets
The experiments use LEVIR-Ship for optical ship detection and SSDD for SAR ship detection. Download the datasets from their official sources:
Dataset	Official repository	
LEVIR-Ship	LEVIR-Ship	Images—COCO release · COCO annotations
SSDD	Official SSDD	Dataset 
https://drive.google.com/file/d/1ItolDrLdSN0R-AnKbD90ngSWMtKOCUaY/view
https://drive.google.com/file/d/1glNJUGotrbEyk43twwB9556AdngJsynZ/view
These download links are provided by the dataset authors. GitHub
Dataset Preparation
Organize the images and COCO-format annotations as follows. This is the project’s prepared directory structure; downloaded archives may require extraction, annotation conversion, or reorganization.
data/
├── LEVIR-Ship-1/
│   ├── images/
│   │   ├── train2017/
│   │   └── val2017/
│   └── annotations/
│       ├── instances_train2017.json
│       └── instances_val2017.json
└── SSDD/
    ├── images/
    │   ├── train/
    │   └── test/
    └── annotations/
        ├── train.json
        └── test.json

Both datasets use a single detection category, ship, with horizontal bounding-box annotations. Image paths and annotation filenames must match the dataset configuration.
Code Availability
The source code will be made publicly available in this repository after publication of the paper.
