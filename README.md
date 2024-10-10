```
💡 The best goal is the one that you can stick to.
--------------------------------------------------
🟥 CONVOLUTIONAL NEURAL NETWORK (CNN)
└── ...
🟩 OBJECT DETECTION
├── 🟥 GENERIC OBJECT DETECTION
│   ├── [CVPR] Can we trust bounding box annotations for object detection, Jeffri Murrugarra-Llerena, 2022
│   │   ├── (Keywords) Oct9-24, horizontal bbox (HBB), oriented bbox (OBB), bbox annotation discrepancy
│   │   ├── (Problem Statement)
│   │   │   ├── BB annotation is not an objective process, especially for occluded object.
│   │   │   │   └── (should we annotate the occluded part?)
│   │   │   └── Discrepancy in annotating might significantly impact the IOU and mAP.
│   │   ├── (Method)
│   │   │   ├── The annotation consistency is determined by comparing annotated BB and segmentation mask BB.
│   │   │   │   └── (This will emulate the human error between 2 annotators)
│   │   │   └── The relationship between IOU and BB dimension is determined by category-agnostic scatter plot.
│   │   └── (Findings)
│   │       ├── Even sub-pixel discrepancies (i.e., 1 pixel difference) between AHBBs and SHBBs ...
│   │       │   └── can lead to strong IoU degradations, particularly for small objects.
│   │       ├── The effect on IOU is dependent on BB size (especially for small BB).
│   │       ├── Small and medium objects are more susceptible to sub-pixel errors than large objects.
│   │       └── Discrepancies between direct AOBBs and SOBBs are deeper than HBB annotations.
│   ├── [IJCV] Deep Learning for Generic Object Detection: A Survey, Li Liu, 2019
│   └── [axXiv] How Trustworthy are Performance Evaluationsfor Basic Vision Tasks?, Tran Thien Dat Nguyen, 2022
├── 🟩 SMALL OBJECT DETECTION (SOD)
│   └── ...
└── 🟦 ORIENTED BOUNDING BOX (OBB)
    └── ...
🟦 DATASET
├── [CVPR] Imagenet: A large-scale hierarchical image database, J Deng, 2009
├── [IJCV] The PASCAL Visual Object Classes (VOC) Challenge, Mark Everingham, 2010
├── [ECCV] Microsoft COCO: Common Objects in Context, Tsung-Yi Lin, 2014
└── [CVPR] Are we ready for Autonomous Driving? The KITTI Vision Benchmark Suite, Andreas Geiger, 2012
🟨 NICHE
└── [Commun. ACM] Determining the minimum-area encasing rectangle for an arbitrary closed curve, H. Freeman, 1975
    ├── (Keywords) 
    └── (Problem Statement)
        ├── original: How to fit a minimum-area bounding rectangle to the shape?
        └── interpreted: How to extract oriented BB automatically from segmentation masks?
```