This project is Tiger Image Recognition built specifically for Raspberry Pi.


## Demo Video

[Youtube Video](https://www.youtube.com/watch?v=xbodrDBD4TU&t=30s&ab_channel=SujayAlaspure)

## Libraries Required

- OpenCV [Link for Installation on Pi](https://www.pyimagesearch.com/2018/09/26/install-opencv-4-on-your-raspberry-pi/?fbclid=IwAR07vEjKD_AdD-xlshi37vQhWN8J7nlAWVKf8JRQ38ktlV6jgoKn6W2nf2Q)
- Numpy
- Argparse (built in)
- Time (built in)
- Os (built in)
- Shutil (built in)

## How to run on Raspberry Pi:

Open Terminal and enter the below commands

```
Source ~/.profile
Workon cv
Python [filename]
```

## To run on Laptop

Run below command from terminal.:(Same Directory)

```Bash
Python deepl.py
```

### To Change picture make changes to line 22 & 23 in `deepl.py`:

```Python
img_org = "images/" #Path to image Directory w. r. to source directory
img_name = "tig9.jpg" # Image Name
```

### To change picture everytime through CLI

```
Python deep_learning.py --image [image_path_from_source_directory]
```

### Output:

When you run the program the image you given the input to the code will be copied to the another folder Path:
tig > for Run1
tig/image > for Run2

### To change the destination folder change line 58 :

`shutil.copy2(img_org + img_name, "tig/" + img_name)`

Syntax: shutil.copy2(source, Destination)

### To display ON OFF output image toggle comment the line 64:

`cv2.imshow("Image", image)`

## Ref

https://www.pyimagesearch.com/2017/08/21/deep-learning-with-opencv/
