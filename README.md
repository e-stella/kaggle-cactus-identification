# kaggle-cactus-identification
Determining whether an aerial image contains a columnar cactus

Skeleton
kaggle-cactus-identification/
│
├── README.md
├── .gitignore
│
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_data_preparation.ipynb
│   ├── 03_baseline_cnn.ipynb
│   ├── 04_transfer_learning.ipynb
│   └── 05_inference_submission.ipynb
│
├── src/
│   ├── __init__.py
│
│   ├── config.py
│
│   ├── data/
│   │   ├── __init__.py
│   │   ├── dataset.py        # PyTorch / TF Dataset
│   │   └── transforms.py     # Augmentations
│   │
│   ├── models/
│   │   ├── __init__.py
│   │   ├── cnn.py
│   │   ├── resnet.py
│   │   └── efficientnet.py
│   │
│   ├── training/
│   │   ├── __init__.py
│   │   ├── train.py
│   │   ├── validate.py
│   │   └── losses.py
│   │
│   ├── inference/
│   │   └── predict.py
│   │
│   └── utils/
│       ├── seed.py
│       ├── metrics.py
│       └── logger.py
│
├── experiments/
│   ├── exp001_baseline.yaml
│   ├── exp002_resnet.yaml
│   └── exp003_effnet_aug.yaml
│
├── data/              # gitignored
│   ├── train/
│   ├── test/
│   └── train.csv
│
├── models/            # gitignored
│   └── checkpoints/
│
├── output/            # gitignored
│   ├── submissions/
│   └── logs/
│
└── submission/
    └── sub_baseline.csv
