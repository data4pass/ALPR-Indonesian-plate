# ALPR-Indonesian-plate

An ALPR (Automatic License Plate Recognition) program for Indonesian plate numbers. Forked from [ALPR-Indonesian-plate](https://github.com/muchlisinadi/ALPR-Indonesian-plate) by [muchlisinadi](https://github.com/muchlisinadi/ALPR-Indonesian-plate).

## Usage
`python Main.py -c directoryFileImage`  Calibrate camera and threshold.

`python Main.py`  Use with camera.

`python Main.py -i /path/to/image` Recognize an image.

`python Main.py -v /path/to/video` Recognize a video.


## Retrain training data
`python GenData.py -d /train_image/train2.png` where `train2.png` is the image used for the training.

The training will produce two outputs: `classifications.txt` and `flattened_images.txt`.

Press `esc` to cancel and exit the training.

## Check if the classification is good enough
    python TrainAndTestData.py -d = train_image/train2.png

## Invert an image
    python invert_imageData.py -d = train_image/train2.png