# ALPR-Indonesian-plate

An ALPR (Automatic License Plate Recognition) program for Indonesian plate numbers. Forked from [ALPR-Indonesian-plate](https://github.com/muchlisinadi/ALPR-Indonesian-plate) by [muchlisinadi](https://github.com/muchlisinadi/ALPR-Indonesian-plate).

## Usage
`python2 Main.py -c path/to/image`  Calibrate image.

`python2 Main.py`  Use with camera.

`python2 Main.py -i path/to/image` Recognize an image.

`python2 Main.py -v path/to/video` Recognize a video.


## Retrain training data
`python2 GenData.py -d train_image/train2.png` where `train2.png` is the image used for the training.

The training will produce two files: `classifications.txt` and `flattened_images.txt`.

Press `Esc` to cancel and exit the training.

## Check if the classification is good enough
    python2 TrainAndTestData.py -d train_image/train2.png

## Invert an image
    python2 invert_imageData.py -d train_image/train2.png