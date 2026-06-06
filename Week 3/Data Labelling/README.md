# Dataset Labeling

In this phase, we will create a labeled dataset that will be used to train the Conditional GAN in later stages of the project.

## Objectives

* Create a clean and structured dataset suitable for conditional image generation.
* Use only a small set of simple and interpretable labels.
* Ensure the dataset remains manageable in size while being large enough to train a meaningful model.
* Use only safe-for-work images.
* Source datasets exclusively from Kaggle.

## Labeling Guidelines

To keep the project focused and computationally feasible, use only basic visual attributes such as:

* Hair Color
* Eye Color
* Hair Length
* Expression (optional)

Avoid highly specific or rare tags, character names, franchise names, or complex scene descriptions.

Examples of suitable labels:

```text
blue_hair
black_hair
pink_hair
brown_hair
blonde_hair

blue_eyes
red_eyes
green_eyes
brown_eyes
```

## Dataset Structure

Organize the dataset as follows:

```text
dataset/
├── images/
│   ├── 0001.jpg
│   ├── 0002.jpg
│   └── ...
└── labels.csv
```

The corresponding labels file should follow the format:

```csv
image,hair
0001.jpg,blue_hair
0002.jpg,black_hair
0003.jpg,pink_hair
```

For multiple attributes:

```csv
image,hair,eyes
0001.jpg,blue_hair,red_eyes
0002.jpg,black_hair,brown_eyes
0003.jpg,pink_hair,green_eyes
```

## Label Acquisition

Labels may be obtained using either of the following approaches:

### Option 1: Extract Existing Labels

Use datasets that already contain tags or annotations and extract only the attributes relevant to the project.

### Option 2: Create Custom Labels

Manually label a subset of images if suitable annotations are unavailable.

For this project, extracting labels from existing tagged datasets is preferred.

## Dataset Size

The final dataset should:

* Be large enough to learn meaningful visual patterns.
* Remain small enough to train within available computational limits.
* Maintain balanced representation across label categories.

A target range of approximately 10,000–50,000 images is recommended, depending on available hardware.

## Recommended Datasets

### SafeBooru (Pre-Labeled)

https://www.kaggle.com/datasets/alamson/safebooru

Advantages:

* Contains existing tags.
* Suitable for automatic label extraction.
* Large collection of safe images.

### Anime Face Dataset (Unlabeled)

https://www.kaggle.com/datasets/splcher/animefacedataset/data

Advantages:

* Clean anime face images.
* Good starting point for custom labeling.

## Final Deliverable

At the end of this stage, the dataset should consist of:

* A curated image collection.
* A corresponding labels.csv file.
* Consistent and balanced labels.
* Safe-for-work images only.

This dataset will serve as the primary training data for the Conditional GAN developed in subsequent phases of the project.
