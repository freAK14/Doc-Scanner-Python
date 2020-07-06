# Doc-Scanner-Python
Document Scanner using OpenCV

## How to use:

* Run the script 

```
python docscanner.py
```
* Select the image you want to get scanned. 

## What it does ?
The script takes an image as input using the dialog box and then scans the document from the image by applying few image processing techniques and gives the output image with scanned effect

## How does it do this?
Initially we need to resize the images so OpenCV can handle it(since images captured by mobile phones are usually very hize in resolution)and then the following functions are applied:
* Guassian Blur to smoothen image.
* Canny Edges to detect the edges.
* Find contours and boundary of the page.
* Map the end points of contours to 960*720 window.
* Apply perspective transform to get scanned or bird eye view of the image.

## Requirements

* OpenCV
* tkinter
* NumPy

## References

* Official OpenCV documentations and tutorials: https://docs.opencv.org/3.1.0/d6/d00/tutorial_py_root.html
* Article on guassian Blur: https://computergraphics.stackexchange.com/questions/39/how-is-gaussian-blur-implemented
* Aditya Pai's Github Repository: https://github.com/AdityaPai2398/CamScanner-In-Python
