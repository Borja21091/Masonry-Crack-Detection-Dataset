# Masonry Crack Detection Dataset

The dataset contained in this repository is a collection of crack images and their annotated bounding-box annotations. Currently, the dataset only accounts for 'Crack' defects, although it could be expanded in the future. The dataset was targeted to **detection** tasks, hence the bounding-boxes.

# Images

3,291 images of size 224 x 224 pixels.

# Labels

The bounding-box labels are structured following the format used for YOLO format. Each image in the dataset has a corresponding '.txt' file containing the objects in the image. The text files are formatted as:

`<class-id> <x-center> <y-center> <width> <height>`

- <class-id>: integer representing the class of the object. This should start from 0 and increase by 1 for each new object class. This dataset only contains 'Crack' images, therefore `<class-id>` is always 0. In the event of adding more defects, this will be updated accordingly.

- **<x/y-center>**: coordinates of the bounding-box centre, normalised by the width and height of the image. Values should range within [0,1].

- **<width/height>**: dimensions of the bounding-boxes, normalised by the width and height of the image. Values should range within [0,1].
