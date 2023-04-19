# Masonry Crack Detection Dataset

The dataset contained in this repository is a collection of crack images and their annotated bounding-box annotations. Currently, the dataset only accounts for 'Crack' defects, although it could be expanded in the future. The dataset was targeted to ***detection** tasks, hence the bounding-boxes.

# Images

3,291 images of size 224 x 224 pixels.

# Labels

The bounding-box labels are structured following the format used for YOLO format. Each image in the dataset has a corresponding '.txt' file containing the objects in the image. The text file has the format:

> <class-id> <x-center> <y-center> <height> <width>
