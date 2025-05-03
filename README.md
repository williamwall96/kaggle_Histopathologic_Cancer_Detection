# kaggle_Histopathologic_Cancer_Detection

The goal of this project is to detect metastatic cancer in histopathologic images, as part of the Kaggle Histopathologic Cancer Detection Challenge. The task involves developing a classification model that can identify whether a small image patch extracted from a larger histology scan contains tumor tissue.

Each image in the dataset is a 96x96 pixel color image (RGB) in .tif format. The key prediction target is binary:

- label = 1 if the center 32x32 region contains tumor tissue

- label = 0 otherwise

The training dataset includes:

- train_labels.csv: over 220,000 labeled image IDs with binary labels

- train/: corresponding .tif image patches

The test dataset includes:

- test/: ~57,000 unlabeled .tif image patches for final prediction

The task is a binary classification problem using deep learning techniques on image data. The challenge also simulates a real-world medical imaging problem, where accurate classification is essential for downstream diagnosis.

To address this problem, we built and evaluated several convolutional neural network (CNN) architectures, tuned hyperparameters, and ultimately selected a best-performing model to generate predictions for the Kaggle test set.
